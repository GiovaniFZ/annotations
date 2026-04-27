# DOM
- Document Object Model:
- É Toda parte do HTML porém do lado do JavaScript. dessa forma é possível interagir com o HTML (colocando eventos, alterando dados).

# Virtual DOM
- Cópia do DOM que é mantido pelo React em memória.
- Antes de recarregar a página, o React carrega o VirtualDOM e compara com o que já estava na página (Diffing).
- Com isso, temos o reconcilliation: Ele atualiza apenas o que foi alterado na página com uma performance muito boa.

# Render tree
- É usada pelo navegador para renderizar os elementos na tela depois que o diffing e reconcilliation já foi feito.
- Permite que os dados sejam enviados de cima pra baixo