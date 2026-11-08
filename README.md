# Decibéis do Salão

App simples para anotar as medições de decibéis (dB) do Salão de Assembleia:

- **Lado esquerdo:** 3 medições
- **Lado direito:** 3 medições
- **Meio, ao fundo:** 1 medição

Depois de salvo, um registro não pode ser editado nem apagado pelo app. Os registros são exportados em PDF, com a opção de todos ou de um mês.

## Como usar

Abra o `index.html` no navegador, ou use o link do GitHub Pages se estiver ativado.
As medições ficam salvas no próprio navegador do aparelho (localStorage). Use sempre o mesmo aparelho e navegador, e exporte o PDF regularmente como cópia de segurança.

Funciona sem internet depois de aberto: o gerador de PDF ([jsPDF](https://github.com/parallax/jsPDF) 2.5.1, licença MIT) está incluído no projeto.
