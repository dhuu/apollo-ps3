<div align="center">
  <h1>🎮 Ativador de Conta PS3 (Fake/Console)</h1>
  <p>Uma ferramenta super leve e automatizada para ativação instantânea de contas offline no PlayStation 3.</p>

  [![Build Package](https://github.com/dhuu/ativador-conta-ps3/actions/workflows/build.yml/badge.svg)](https://github.com/dhuu/ativador-conta-ps3/actions)
  [![License](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://github.com/dhuu/ativador-conta-ps3/blob/master/LICENSE)
</div>

---

## 💡 O que é?

O **Ativador de Conta PS3** é um utilitário focado exclusivamente em resolver o problema de ativação de contas no PlayStation 3 (criação do arquivo `act.dat`) de forma **100% automatizada e offline**. 

Ele foi construído a partir do incrível código-fonte do *Apollo Save Tool*, porém passando por um processo intenso de otimização e enxugamento. Removemos toda a interface gráfica de gerenciamento de saves, músicas, submenus complexos e digitação manual em teclados virtuais. O resultado é uma ferramenta extremamente rápida que faz apenas o que importa em questão de segundos.

## ✨ Recursos Exclusivos

- 🚀 **One-Click Activation**: Ao iniciar o aplicativo pela XMB, o fluxo de ativação é disparado imediatamente.
- 🪟 **Bypass de Menus**: Nenhuma interface gráfica pesada para navegar. Apenas um pop-up nativo e limpo do PS3 perguntando se você deseja confirmar a ativação.
- ⌨️ **Sem Teclado Virtual (OSK)**: O ID da conta (Account ID) é gerado e injetado nativamente no `xRegistry.sys` debaixo dos panos, sem interromper o usuário pedindo para digitar números.
- 🪶 **Peso Pluma**: Remoção de mais de 60 imagens, dezenas de áudios e arquivos pesados (`appdata.zip`). O pacote final (`.pkg`) é focado exclusivamente no código de ativação.
- 🌙 **Background Elegante**: Mantém a estética original renderizando a logo do aplicativo suavemente ao fundo enquanto a janela do sistema aguarda sua confirmação.

## 📥 Como Baixar e Instalar

1. Vá até a aba **[Releases](https://github.com/dhuu/ativador-conta-ps3/releases)** deste repositório.
2. Baixe a versão mais recente do arquivo `ativar-conta-ps3.pkg`.
3. Coloque o `.pkg` na raiz de um pen-drive formatado em `FAT32` (MBR).
4. No seu PS3, com o HEN ou CFW ativado, vá em `Package Manager` -> `Install Package Files` -> `Standard` e instale o pacote.
5. Inicie o aplicativo direto pela tela inicial (XMB), aperte em "Sim" e pronto! A conta está ativada.

## ⚙️ Como Compilar você mesmo

Este repositório possui Integração Contínua (CI) usando **GitHub Actions**. Isso significa que se você fizer um *fork* deste repositório, o próprio GitHub irá compilar o arquivo `.pkg` para você automaticamente sempre que houver uma alteração no código.

Caso você seja um desenvolvedor e deseje compilar manualmente na sua máquina, você precisará do **PSL1GHT SDK** instalado:
```bash
make pkg
```

## 🤝 Créditos e Agradecimentos

Este projeto só foi possível graças aos esforços brilhantes da comunidade homebrew do PS3:
- Construído e derivado do projeto de código-aberto **[Apollo Save Tool](https://github.com/bucanero/apollo-ps3)** criado por Damian Parrino (**@bucanero**). O motor de ativação interno pertence inteiramente ao Apollo.
- Compilado utilizando o ambiente **PSL1GHT SDK**.
