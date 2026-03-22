# Base de Conhecimento

## Dados Utilizados

| Arquivo | Formato | Para que serve o Mario? |
|---------|---------|---------------------|
| `historico_atendimento.csv` | CSV | Contextualizar interações anteriores. |
| `perfil_investidor.json` | JSON | Personalizar explicações sobre dúvidas e necessidades. |
| `produtos_financeiros.json` | JSON | Conhecer produtos disponíveis a fim de ensiná-los ao usuário. |
| `transacoes.csv` | CSV | Analisar padrão de gastos do cliente a fim de utilizá-los de forma didática. |

---

## Adaptações nos Dados

> Você modificou ou expandiu os dados mockados? Descreva aqui.

Nenhum dado foi modificado.

---

## Estratégia de Integração

### Como os dados são carregados?
> Descreva como seu agente acessa a base de conhecimento.

Duas possibilidades: injetar diretamente os dados no prompt (Ctrl + c, Ctrl + v), ou carregar os arquivos via código, como no exemplo abaixo.

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

Os dados são "injetados" no prompt, garantindo que o agente tenha o melhor contexto possível. Em situações mais robustas, o ideal será carregar dinamicamente.

---

## Exemplo de Contexto Montado

> Mostre um exemplo de como os dados são formatados para o agente.

```
Dados do Cliente:
- Nome: João Silva
- Perfil: Moderado
- Saldo disponível: R$ 5.000

Últimas transações:
- 01/11: Supermercado - R$ 450
- 03/11: Streaming - R$ 55
...
```
