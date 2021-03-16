# Desafio ToDo

## :computer: Sobre o desafio

O desafio consiste em manipular estados no React, seguindo as seguintes funções:

- Adicionar uma nova tarefa.
- Remove uma tarefa
- Marcar e desmarcar uma tarefa como concluida.

### Especificação dos testes

#### Teste TaskList.spec.tsx
- **should be able to add a task** <br />
Para que esse teste passe, deve ser permitido que uma task seja criada e com isso, exibida em tela. As tasks criadas devem conter os atributos seguindo o padrão da interface, que é:

```ts
interface Task {
  id: number;
  title: string;
  isComplete: boolean;
}
```

- **should not be able to add a task with an empty title** <br />
Para que esse teste passe, antes de criar uma nova task, deve ser validado se algo foi digitado no input e não permitir a criação da task caso o valor seja vazio, caso o valor digitado seja vazio, deve ser impedido a criação da task.

- **should be able to remove a task** <br />
Para que esse teste passe, deve ser permitido que ao clicar no botão com ícone de uma lixeira, a task relacionada a esse botão seja removida do estado da aplicação, consequentemente sendo removida da tela.

- **should be able to check a task** <br />
Para que esse teste passe, deve ser permitido que ao clicar no checkbox ao lado da task, ela seja marcada como concluída ou não concluída de acordo com seu estado atual, alterando seu valor de `isComplete` de `false` para `true` ou ao contrário, de `true` para `false`. 

## :clapper: Execução
- Instale as bibliotecas utilizando `npm install` ou qualquer outro gerenciador de pacotes.
- Execute utilizando `npm run dev`. 
- Para realizar os testes, execute `npm run test`.
