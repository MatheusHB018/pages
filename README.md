# 🧮 Calculadora de Análise Combinatória

Uma ferramenta educacional interativa para resolver problemas de análise combinatória, desenvolvida com HTML, CSS e JavaScript puro.

## ✨ Características

- **Modo Guiado (Wizard)**: Auxilia usuários a identificar o método correto através de perguntas sequenciais
- **Modo Direto**: Permite acesso rápido a todos os métodos para usuários avançados
- **Cálculos Precisos**: Implementa todas as fórmulas baseadas no documento "Análise combinatória - notas de aula.pdf"
- **Interface Intuitiva**: Design limpo e responsivo com explicações detalhadas
- **Resultados Completos**: Mostra fórmula, cálculo passo a passo e resultado final

## 📚 Métodos Implementados

| Método | Fórmula | Aplicação |
|--------|---------|-----------|
| Princípio da Adição | m + n | Eventos mutuamente exclusivos (OU) |
| Princípio da Multiplicação | n₁ × n₂ × ... | Eventos em sequência (E) |
| Permutação Simples | P(n) = n! | Organizar todos os elementos (ordem importa) |
| Arranjo Simples | A(n,k) = n!/(n-k)! | Organizar parte dos elementos (ordem importa) |
| Combinação Simples | C(n,k) = n!/(k!(n-k)!) | Selecionar parte dos elementos (ordem não importa) |
| Permutação com Repetição | P(n;n₁,n₂,...) = n!/(n₁!n₂!...) | Organizar elementos com repetições |
| Combinação com Repetição | CR(n,k) = C(n+k-1,k) | Selecionar elementos com repetição |
| Permutação Circular | PC(n) = (n-1)! | Organizar elementos em círculo |

## 🚀 Como Usar

### Modo Guiado (Recomendado para Iniciantes)

1. Clique em "Modo Guiado"
2. Responda as perguntas sequenciais:
   - Identifique se é sequência (E) ou exclusivo (OU)
   - Determine se a ordem importa
   - Verifique se usa todos os elementos
   - Identifique se há repetições
3. A calculadora indicará o método correto
4. Preencha os parâmetros necessários
5. Veja o resultado detalhado

### Modo Direto (Para Usuários Avançados)

1. Clique em "Modo Direto"
2. Selecione diretamente o método desejado
3. Preencha os parâmetros necessários
4. Obtenha o resultado com explicação completa

## 🎯 Fluxo de Decisão do Wizard

P1: Eventos em sequência (E) ou exclusivos (OU)?
├── Sequência/E → Princípio da Multiplicação
├── Exclusivos/OU → Princípio da Adição
└── Reorganizar grupo → P2

P2: A ordem importa?
├── NÃO importa → P3
└── SIM importa → P4

P3: Elementos podem ser repetidos?
├── NÃO podem → Combinação Simples
└── SIM podem → Combinação com Repetição

P4: Usa TODOS os elementos?
├── SIM, todos → P5
└── NÃO, parte → Arranjo Simples

P5: Existem elementos repetidos?
├── SIM, há repetições → Permutação com Repetição
└── NÃO, distintos → P6

P6: Elementos em círculo?
├── SIM, círculo → Permutação Circular
└── NÃO, linha → Permutação Simples

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica da aplicação
- **CSS3**: Estilização moderna com variáveis CSS e design responsivo
- **JavaScript Vanilla**: Lógica de cálculo e interatividade sem dependências

## 📁 Estrutura do Projeto
calculadora-combinatoria.zip/
│
├── index.html # Arquivo principal HTML
└── README.md # Este arquivo

## 🔧 Funções JavaScript Principais

### Cálculos Matemáticos
```javascript
fatorial(n)              // Calcula n!
principioAdicao(...)     // Soma de eventos exclusivos
principioMultiplicacao(...) // Produto de eventos sequenciais
permutacaoSimples(n)     // P(n) = n!
arranjoSimples(n, k)     // A(n,k) = n!/(n-k)!
combinacaoSimples(n, k)  // C(n,k) = n!/(k!(n-k)!)
permutacaoComRepeticao(n, ...) // P(n;n₁,n₂,...)
combinacaoComRepeticao(n, k)   // CR(n,k)
permutacaoCircular(n)    // PC(n) = (n-1)!


## 📦 Instruções para Download

Para baixar o projeto completo:

1. **Copie o código HTML acima** e salve como `index.html`
2. **Copie o conteúdo do README** e salve como `README.md` 
3. **Compacte os dois arquivos** em um ZIP chamado `calculadora-combinatoria.zip`
