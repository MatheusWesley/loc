## Explicação do código

**Código:**
```html
<q-input label="Nome" outlined>
  <template v-slot:append>
    <q-icon name="person" class="cursor-pointer">
    </q-icon>
  </template>
</q-input>
```

- q-input
Aqui basicamente estou usando o componente q-input que é equivalente ao input do HTML.
Label: Essa propriedade estou definindo o nome que vai ser mostrado no input
outlined: é a estilização do quasar que da esse efeito com a borda no input

- template
Nessa parte eu vou colocar o ícone do input, eu preciso colocar dentro de uma tag <template>
porque ela me permite usar a propriedade _v-slot:append_ que em linhas gerais significam:
    - v-slot: Esta diretiva indica que estamos definindo um slot.
    - append: Este é o nome do slot. Ele indica que o conteúdo dentro deste template será inserido na posição final do componente pai onde o slot foi definido.

Ou seja, estou dizendo que onde o ícone ficará

- q-icon
Aqui estou colocando o ícone
name: coloco o nome do ícone que quero usar do quasar
nesta classe informa que ao colocar o mouse por cima ele vai ficar com uma mãozinha



