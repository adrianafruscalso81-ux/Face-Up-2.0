# FaceUp 2.0 — versão para gerar APK

Este pacote transforma o FaceUp 2.0 (que já é um PWA) em um aplicativo Android usando Capacitor.

## O que foi preparado
- `www/` — seu aplicativo original.
- `package.json` — dependências do Capacitor.
- `capacitor.config.json` — nome, ID e pasta do aplicativo.
- `.github/workflows/build-apk.yml` — o GitHub Actions gera automaticamente um APK de teste.

## Como usar no GitHub
1. Extraia este ZIP.
2. No repositório do GitHub, envie **os arquivos e pastas de dentro deste ZIP**, e não o ZIP inteiro.
3. Abra a aba **Ações** (Actions).
4. Abra **Gerar APK do FaceUp 2.0**.
5. Toque em **Run workflow / Executar fluxo de trabalho**.
6. Quando terminar, abra a execução concluída e baixe o artefato **FaceUp-2.0-APK**.
7. Dentro dele estará `app-debug.apk`, que pode ser instalado no seu Android.

O APK gerado é para uso pessoal/teste e não é assinado para publicação na Play Store.

## Observação
O aplicativo original usa Tailwind, Lucide e canvas-confetti por CDN, então algumas funções visuais ainda dependem de internet na primeira abertura.
