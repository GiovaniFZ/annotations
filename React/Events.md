# Diferenças entre eventos JS vanilla e React
- Vanilla:
```js
<button onclick="handleClick()" />
```
- React
```js
<button onClick={handleClick()} />
```

- SynteticEvent: É um encapsulador sobre os eventos nativos do navegador no React. Garante que os eventos funcionem de forma consistente em diversos navegadores para melhorar a eficiência da performance.
- Event Delegation: É o gerenciador de eventos (quem vai colocar os "onClick, onSubmit" no botão). Ele também faz a limpeza de eventos automaticamente.
- AddEventListener: Usar como última opção. (Um exemplo prático seria utilizar para eventos no body, para deixar dark ou light). Lembrar de destruir o evento quando destruir o componente (ciclo de vida);