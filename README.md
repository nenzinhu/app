# PMRv 4em1 — iOS Build

Projeto isolado para geração do `.ipa` no **Codemagic** (sem precisar de Mac).

## Estrutura
```
PMRV-4em1-iOS/
├── www/
│   └── index.html        ← App web principal
├── resources/
│   ├── icon-only.png     ← Ícone do app
│   └── splash.png        ← Splash screen
├── capacitor.config.json ← Configuração Capacitor iOS
├── package.json          ← Dependências (apenas iOS)
├── codemagic.yaml        ← Pipeline de build na nuvem
└── *.png                 ← Imagens usadas no app
```

## Como gerar o IPA

1. **Suba esta pasta no GitHub** (crie um repositório novo)
2. **Acesse** [codemagic.io](https://codemagic.io) e conecte o repositório
3. Adicione seu **Apple ID** em Teams → Integrations → Developer Portal
4. No `codemagic.yaml`, substitua `seu-email@exemplo.com` pelo seu e-mail
5. Inicie o build — o `.ipa` fica disponível para download

## Instalar o IPA no iPhone (sem App Store)
- [Sideloadly](https://sideloadly.io) — mais simples, requer iTunes no PC
- [AltStore](https://altstore.io) — alternativa gratuita

> Com Apple ID gratuito, o app expira em 7 dias.
> Com Apple Developer ($99/ano), o app não expira.
