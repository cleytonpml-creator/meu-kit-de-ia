# Template de Delegação: Fechamento Diário de Rota e Conciliação (Londres - UK)

## Objetivo
Consolidar os números brutos do turno de entregas em Londres, calcular o rendimento líquido por hora após custos operacionais da van (Ford Transit Custom) e identificar gargalos na rota para o dia seguinte.

## Contexto
- **Operação:** Motorista autônomo de entregas (courier EVRi) atuando na região de Edmonton / Norte de Londres (postcodes N9, N18, E4).
- **Dispositivo:** Execução mobile-first via Google Pixel 11 Pro XL ao final do expediente.
- **Regra de Privacidade (GDPR):** Nenhum dado pessoal de destinatário, endereço exato ou placa real é enviado neste fluxo.

## Recursos / Dados de Entrada
- Quantidade total de pacotes manifestados vs. entregues com sucesso.
- Quantidade e motivo de devoluções (*Returns / RTS*).
- Duração total do turno (início no depósito até a última baixa).
- Gasto estimado com diesel no dia e eventuais taxas (ex: estacionamento pago).

## Limites e Critérios de Sucesso
1. **Não inventar números:** Se faltar algum dado (como consumo médio de diesel ou tarifa), pergunte antes de calcular.
2. **Separação Fato vs. Sugestão:** Divida a entrega em dois blocos claros: *Dados Confirmados* e *Sugestões de Otimização*.
3. **Aprovação Obrigatória:** Apresente primeiro o plano de execução e aguarde o meu "OK" antes de gerar o relatório final.

## Prompt Pronto para Uso

```text
Quero delegar a você o fechamento e análise do meu turno de entregas hoje em Londres (região de Edmonton).

- Objetivo: Gerar o resumo financeiro/operacional do dia e apontar melhorias para a próxima rota.
- Dados do turno de hoje: [Cole aqui: pacotes entregues, devoluções, horas trabalhadas, gasto com diesel]
- Regras obrigatórias:
  1. Não invente nenhuma tarifa, valor de combustível ou regra de trânsito; se faltar dado, me pergunte.
  2. Separe explicitamente o que são fatos informados por mim do que são sugestões suas.
  3. Antes de gerar o relatório final, me mostre o plano de como você vai organizar os cálculos e aguarde minha aprovação.
