# Pilha Encadeada em C

Este projeto implementa uma **pilha encadeada** em **C**, utilizando **listas ligadas** para armazenar elementos dinamicamente. A pilha segue o princípio **LIFO (Last In, First Out)**, onde o último elemento inserido é o primeiro a ser removido.

## 📚 Estrutura da Pilha

A pilha é composta por três estruturas principais:

- **`tdado`**: Representa os dados armazenados na pilha (um site e uma data).
- **`tno`**: Representa um nó da pilha, contendo um dado e um ponteiro para o próximo nó.
- **`tpilha`**: Estrutura que contém um ponteiro para o topo da pilha.

## 🚀 Operações da Pilha

### **Inicialização**
A função `inicializa(tpilha *p)` define o topo da pilha como `NULL`, indicando que está vazia.

### **Inserção (`push`)**
A função `push(tpilha *p, tdado x)`:
- Aloca memória para um novo nó.
- Armazena o dado no nó.
- Ajusta o ponteiro do topo para o novo nó.
- Retorna `1` se a inserção for bem-sucedida ou `0` em caso de erro.

### **Remoção (`pop`)**
A função `pop(tpilha *p)`:
- Armazena o nó do topo em uma variável auxiliar.
- Atualiza o topo para o próximo nó.
- Libera a memória do nó removido.
- Retorna o dado do nó removido.

### **Verificação de Pilha Vazia (`isEmpty`)**
A função `isEmpty(tpilha p)` verifica se o topo da pilha é `NULL`, retornando `1` se estiver vazia e `0` caso contrário.

### **Consulta ao Topo (`peek`)**
A função `peek(tpilha p)` retorna o dado armazenado no topo da pilha sem removê-lo.

### **Exibição da Pilha (`mostraPilha`)**
A função `mostraPilha(tpilha p)` percorre a pilha do topo até o último elemento, exibindo os dados armazenados.

## 🖥️ Exemplo de Uso

1. Inicialize a pilha com `inicializa(&p1);`
2. Insira elementos com `push(&p1, x);`
3. Remova elementos com `pop(&p1);`
4. Consulte o topo com `peek(p1);`
5. Exiba toda a pilha com `mostraPilha(p1);`

## 📌 Observações
- A pilha **não tem tamanho fixo**, pois usa **alocação dinâmica**.
- Cada elemento é armazenado em um **nó**, permitindo manipulação eficiente.
- A estrutura é ideal para **históricos de navegação**, **desfazer ações** e outras aplicações que utilizam pilhas.

---

### 📌 Projeto desenvolvido por **José Carlos Souza** para fins didáticos no **IFSULDEMINAS - Campus Machado**.
