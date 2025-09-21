# 📘 Projeto: Controle de Notas

Este projeto é uma aplicação simples em **TypeScript** que permite
lançar notas de um aluno, calcular a média e exibir se o aluno foi
**Aprovado** ou **Reprovado**.

------------------------------------------------------------------------

## 📂 Estrutura do Projeto

    PROJETOTYPE/
    │
    ├── ControleDeNotas/          # Pasta principal do código fonte
    │   ├── controle.ts           # Classe Controle com atributos, getters/setters e lógica de avaliação
    │   └── main.ts               # Arquivo principal que executa o programa (menu interativo)
    │
    ├── node_modules/             # Dependências instaladas (gerado automaticamente)
    │
    ├── package.json              # Configuração do projeto e dependências
    ├── package-lock.json         # Controle de versões exatas das dependências
    ├── tsconfig.json             # Configuração do compilador TypeScript
    └── README.md                 # Documentação do projeto

------------------------------------------------------------------------

## 🚀 Funcionalidades

1.  **Cadastro de Notas**\
    O usuário pode digitar **quatro notas** (pnota, snota, rnota,
    xnota).

2.  **Cálculo da Média**\
    A média é calculada automaticamente:

        media = (nota1 + nota2 + nota3 + nota4) / 4

3.  **Verificação de Aprovação**

    -   Se a média for **maior ou igual a 60** → ✅ **Aprovado**\
    -   Caso contrário → ❌ **Reprovado**

4.  **Menu Interativo**

    -   `1` → Lançar notas\
    -   `9` → Sair

------------------------------------------------------------------------

## 🛠️ Tecnologias Utilizadas

-   **TypeScript** → Tipagem estática e orientação a objetos.\
-   **Node.js** → Ambiente de execução.\
-   **prompt-sync** → Leitura de dados no terminal.

------------------------------------------------------------------------

## 📥 Instalação e Execução

### 1. Clonar o repositório

``` bash
git clone https://github.com/seu-usuario/ControleDeNotas.git
cd ControleDeNotas
```

### 2. Instalar dependências

``` bash
npm install
```

### 3. Compilar o TypeScript

``` bash
npx tsc
```

### 4. Executar o programa

``` bash
node ControleDeNotas/main.js
```

------------------------------------------------------------------------

## 📌 Exemplo de Execução

    =========Menu=========
    1. Lançar Notas
    9. Sair
    Escolha uma opção: 1
    Digite a primeira nota: 70
    Digite a segunda nota: 80
    Digite a terceira nota: 65
    Digite a quarta nota: 90
    Aprovado

------------------------------------------------------------------------

## 📚 Estrutura da Classe `Controle`

``` ts
export class Controle {
  constructor(
    private _nota1: number,
    private _nota2: number,
    private _nota3: number,
    private _nota4: number,
    private _media: number
  ) {}

  // Getters e setters para as notas e média
  // Método avaliacao calcula a média e mostra o resultado
}
```

------------------------------------------------------------------------

## ✨ Possíveis Melhorias Futuras

-   Implementar armazenamento das notas em arquivo ou banco de dados.\
-   Adicionar mais opções ao menu, como visualizar histórico de notas.\
-   Criar uma interface gráfica simples com HTML/CSS/JS.

------------------------------------------------------------------------

🔖 **Autor:** Seu Nome Aqui\
📅 **Versão:** 1.0
