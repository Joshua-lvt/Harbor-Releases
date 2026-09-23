# Harbor 2.0 — Downloads oficiais

Aplicativo de comunicação peer-to-peer (chamadas, chat, Watch Together, modo Dormir).

> Este repositório **não contém código-fonte**. Ele existe apenas para
> apresentar o Harbor e distribuir as atualizações automáticas.
> Novas versões são compiladas na máquina do mantenedor e publicadas aqui
> como **assets de GitHub Release**.

## Baixar

- **Linux (x86_64):** AppImage com dependências [`harbor-linux-x86_64.AppImage`](https://github.com/Joshua-lvt/Harbor-Releases/releases/latest) — dê permissão de execução e abra
- **Windows (x86_64):** instalador em PT-BR [`harbor-windows-x86_64-setup.exe`](https://github.com/Joshua-lvt/Harbor-Releases/releases/latest) — inclui o WebView2 se necessário
- **Android (x86_64):** [`harbor-android-x86_64.apk`](https://github.com/Joshua-lvt/Harbor-Releases/releases/latest)

Abra a [página da última Release](https://github.com/Joshua-lvt/Harbor-Releases/releases/latest)
e baixe o arquivo da sua plataforma.

## Atualizações automáticas

O próprio Harbor verifica novidades em segundo plano ao abrir:

1. Se não houver nada novo, nada acontece.
2. Se houver, o Harbor pergunta se você quer atualizar (recomendado).
3. Aceitando, ele baixa, instala e reinicia sozinho na nova versão.
   No Android, ele baixa o APK e abre a tela de instalação do sistema.

## Verificação

Cada asset da Release informa `sha256` e `size` no manifesto
[`latest.json`](https://raw.githubusercontent.com/Joshua-lvt/Harbor-Releases/main/latest.json),
e o aplicativo confere o hash antes de instalar.
