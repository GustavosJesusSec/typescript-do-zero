# Aprendizado de TypeScript com Node.js

Este repositório é um registro de prática. A ideia é fazer projetos pequenos, evoluir uma funcionalidade por vez e guardar cada etapa no Git.

## Antes de começar

Instale uma versão LTS recente do Node.js em https://nodejs.org/ e confira:

```sh
node --version
npm --version
```

Depois, nesta pasta:

```sh
npm install --save-dev typescript @types/node
npm run check
npm start
```

O comando `npm start` executa o arquivo TypeScript com o suporte a remoção de tipos do Node.js. O comando `npm run check` verifica os tipos com o compilador TypeScript. Use uma versão LTS recente do Node.js que aceite executar arquivos `.ts` diretamente.

## Projeto 1: lista de tarefas no terminal

Trabalhe em `src/index.ts`, uma etapa por vez:

1. Crie um tipo `Tarefa` com `id: number`, `titulo: string` e `concluida: boolean`.
2. Crie um array `Tarefa[]` com duas tarefas e mostre os títulos no terminal.
3. Escreva `adicionarTarefa(lista, titulo)` para retornar uma nova lista com a tarefa adicionada. Pense no caso da lista vazia.
4. Escreva `concluirTarefa(lista, id)` para retornar uma nova lista com a tarefa marcada como concluída.
5. Escreva `listarPendentes(lista)` e mostre o resultado.
6. Adicione uma regra: título vazio não deve gerar uma tarefa.

Depois de cada etapa, execute `npm run check` e `npm start`. Faça um commit ao concluir uma etapa que funciona.

## Próximos projetos

1. **Entrada pelo terminal:** escolha uma operação com `process.argv`. Aprenda argumentos, validação e uniões de tipos.
2. **Salvar em arquivo JSON:** carregue e grave tarefas com `node:fs/promises`. Aprenda `async`/`await`, tratamento de erros e validação de dados externos.
3. **Testes:** use `node:test` para conferir as regras da lista de tarefas.
4. **API HTTP simples:** exponha as operações com `node:http`. Aprenda requisição, resposta, status e separação de módulos.
5. **Só depois:** experimente um framework e um banco de dados.

## Regra de estudo

Tente sozinho por 25 a 40 minutos. Se travar, leia a mensagem de erro e consulte a documentação. Ao usar IA, peça uma dica ou a explicação do erro, sem pedir a função pronta. No dia seguinte, refaça uma das funções sem olhar o código anterior.

Referências: [TypeScript para novos programadores](https://www.typescriptlang.org/docs/handbook/typescript-from-scratch) e [TypeScript no Node.js](https://nodejs.org/api/typescript.html).
