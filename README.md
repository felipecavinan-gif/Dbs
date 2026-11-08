# Decibéis do Salão

App simples para anotar as medições de decibéis (dB) do Salão de Assembleia:

- **Lado esquerdo:** 3 pontos
- **Lado direito:** 3 pontos
- **Meio, ao fundo:** 1 ponto

Em cada ponto você anota a **mínima** e a **máxima**. O app calcula sozinho a **média de cada ponto** ((mín + máx) ÷ 2), a **média de cada lado** (esquerdo, direito e meio) e a **média geral**, que é a média dessas três médias. Qualquer valor é aceito e campos podem ficar em branco.

Depois de salvo, um registro não pode ser editado nem apagado pelo app. Os registros são exportados em PDF, com a opção de todos ou de um mês.

## Como funciona

- **Autosave:** cada valor é guardado no momento em que é digitado.
- **Backup de reserva:** cada gravação também vai para uma cópia separada no aparelho (localStorage e IndexedDB). Se a lista principal sumir, o app recupera da reserva ao abrir.
- **Botão Salvar medição:** conclui a medição e limpa o formulário para a próxima. Até lá, tudo já fica guardado pelo autosave. Se a página recarregar no meio, o app volta para a medição em andamento. Uma medição esquecida aberta é salva sozinha depois de 30 minutos parada.
- **Exportar PDF:** todos os registros, um mês ou um registro só (botão PDF em cada registro).
- **Apagar:** cada registro tem um botão Apagar, com confirmação antes.

## Como usar

Abra o site pelo GitHub Pages: https://felipecavinan-gif.github.io/Dbs/
As medições ficam no navegador do aparelho. Use sempre o mesmo aparelho e navegador, e exporte o PDF de vez em quando como cópia extra.

O gerador de PDF ([jsPDF](https://github.com/parallax/jsPDF) 2.5.1, licença MIT) está incluído no projeto.
