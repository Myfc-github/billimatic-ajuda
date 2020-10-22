---
title: Importar regras de faturamento via Excel
layout: blog
weight: 4
---
A criação de regras de faturamento pode ser feita através da importação de planilha Excel.

Acesse o menu “Contratos” e clique em “Importar Regras de Faturamento via Excel”.

Faça download da planilha Excel de exemplo, clicando no respectivo link.

![Instruções: Baixe a planilha Exel de exemplo, substitua os dados do exemplo pelos seus (tome o cuidado de não apagar a(s) linha(s) de cabeçalho) e importe.](/images/uploads/importar-regras-de-faturamento-via-excel-1.png "Importar regras de faturamento via Excel - 1")

Abra a planilha. A segunda linha da planilha traz um exemplo de regra de faturamento. Substitua com os dados de suas regras, tomando o cuidado de manter as duas primeiras linhas intactas (que contém o título das colunas).

![Planilha Exel de exemplo](/images/uploads/importar-regras-de-faturamento-via-excel-2.png "Importar regras de faturamento via Excel - 2")

Cada coluna corresponde a uma informação da tela de criação de regra de faturamento. Para saber mais sobre a criação de uma regra, consulte o tópico [Criar nova regra de faturamento](/docs/configuracoes-iniciais/programe-seus-faturamentos/criar-nova-regra-de-faturamento/).

Devem ser informadas as colunas:

Nota: Todas as datas devem ser informadas no formato DD/MM/AAAA, por exemplo 01/07/2020.

* Nome do Contrato - Nome do contrato em que será criada a regra.
* Título da Regra - Corresponde ao campo “Título”, da seção “Informações Gerais” da regra.
* CPF/CNPJ do Cliente - Corresponde ao cliente da seção “Cliente” da regra. Se deixado em branco, a regra herda o mesmo cliente do contrato.
* Serviços - Correspondem aos serviços da seção “Serviços” da regra. Eles devem ser informados respeitando a seguinte sintaxe:

Preencher cada serviço entre colchetes ('\[...]'), com valores separados por ponto-e-vírgula (';'). O formato é: \[Nome do serviço;Descrição do serviço;Quantidade;Valor unitário]

Ex.: Para cadastrar dois serviços:

1. Serviço “Treinamento”, descrição “Treinamento de módulo financeiro”, quantidade 1 e valor unitário R$ 1500,00.
2. Serviço “Consultoria”, descrição “Implantação do módulo fiscal”, quantidade 1 e valor unitário R$ 5500,50.

Deve ser informado:

\[Treinamento;Treinamento de módulo financeiro;1;1500]\[Consultoria;Implantação do módulo fiscal;1;5500,5]

Caso não haja descrição para o serviço, basta não informá-lo. No exemplo anterior o valor informado seria:

\[Treinamento;1;1500]\[Consultoria;1;5500,5]

* Valor bruto - Corresponde ao campo “Valor bruto de cada faturamento”, da seção “Serviços” da regra. Caso tenha informado serviços, ele deve ser deixado em branco, já que seu valor será calculado pela soma dos serviços.
* Data do primeiro faturamento - Corresponde ao campo “Criar o primeiro faturamento em” da seção “Faturamento” da regra.
* Repetir a cada n meses - Corresponde ao campo “repetindo-o” da seção “Faturamento” da regra. Deve ser informado o número de meses, ou deixado em branco, para periodicidade semanal. Por exemplo, para periodicidade mensal, informar 1. Já para anual, informar 12.
* Data do último faturamento - Corresponde ao campo “até o dia”, da seção “Faturamento” da regra.
* Descrição do Faturamento - Corresponde ao campo “Descrição” da seção “Faturamento” da regra.
* Tipo de faturamento - Corresponde ao campo “Tipo de faturamento” da seção “Faturamento” da regra. Devem ser informados os valores Manual ou Automático.
* Modelo de e-mail para notificação automática - Corresponde ao campo “Modelo de Notificação Automática” da seção “Faturamento” da regra. Deve ser informado o nome do modelo de notificação, somente para faturamentos automáticos.
* Competência - Corresponde ao campo “Competência” da seção “Faturamento” da regra. Deve ser informado No mesmo mês ou No mês anterior. Se não informado, assume o valor No mesmo mês.
* Dia do mês - Se informado, aplica a opção de vencimento 'No próximo dia n após a data do faturamento”. Deve ser informado o dia do mês.
* Após n meses - Se informado, em combinação com a informação “Dia do mês”, aplica a opção de vencimento “No dia m após n mes(es) da data do faturamento”. Deve ser informado o número de meses.
* Após n dias úteis - Se informado, aplica a opção de vencimento “Após n dias úteis da data do faturamento”. Deve ser informado o número de dias úteis.
* Após n dias corridos - Se informado, aplica a opção de vencimento “Após n dias corridos da data do faturamento”. Deve ser informado o número de dias corridos.
* Se as colunas “Dia do mês”, “Após n meses “, “Após n dias úteis” e “Após n dias corridos” não forem informadas, aplica a opção de vencimento “No último dia do mês da data do faturamento”.
* Número de parcelas - Se informado, habilita a opção “Dividir em n parcelas iguais”.
* Data do primeiro reajuste - Corresponde ao campo “Primeiro reajuste”, da seção “Configurações de reajuste automático” da regra.
* Periodicidade do reajuste (meses) - Corresponde ao campo “Periodicidade de reajuste”, da seção “Configurações de reajuste automático” da regra.
* Índice do reajuste - Corresponde ao campo “Índice”, da seção “Configurações de reajuste automático” da regra. Devem ser informados os valores: IPCA, IGP-M, IGP-DI, INPC ou IPC-Fipe.
* Notificação do reajuste (dias) - Corresponde ao campo “Notificação (dias)”, da seção “Configurações de reajuste automático” da regra.
* Modelo de NFS-e (Emites) - Corresponde ao campo “Modelo de NFS-e (Emites)”, da seção “Nota fiscal” da regra. Deve ser informado o nome do modelo.
* Corpo da NFS-e - Corresponde ao campo “Corpo da NFS-e”, da seção “Nota fiscal” da regra.
* Dias para emissão da NFS-e após o recebimento - Se informado, aplica a opção “Após n dia(s) útil(eis) do recebimento”, da seção “Nota fiscal” da regra. Caso não seja informado, aplica a opção “No dia do faturamento”.
* Forma de pagamento - Corresponde ao campo “Forma de pagamento”, da seção “Cobrança” da regra. Devem ser informados Boleto bancário, Cartão de crédito ou Transferência bancária.
* Configuração de cobrança (Cobrato) - Corresponde ao campo “Configuração de cobrança (Cobrato)”, da seção “Cobrança” da regra. Deve ser informado o nome da configuração de cobrança.
* Modelo de cobrança (Cobrato) - Corresponde ao campo “Modelo de cobrança (Cobrato)”, da seção “Cobrança” da regra. Deve ser informado o nome do modelo de cobrança.
* Categoria (Myfinance) - Corresponde ao campo “Categoria”, da seção “Financeiro (Myfinance)” da regra. Deve ser informado o nome da categoria.
* Centro de receita (Myfinance) - Corresponde ao campo “Centro de receita”, da seção “Financeiro (Myfinance)” da regra. Deve ser informado o nome do centro de receita.
* Conta de recebível (Myfinance) - Corresponde ao campo “Conta de recebível”, da seção “Financeiro (Myfinance)” da regra. Deve ser informado o nome da conta de recebível.

De volta ao Billimatic, selecione o arquivo Clique em “Importar Regras de Faturamento”.

![Imagem de confirmação de que a importação foi concluída.](/images/uploads/importar-regras-de-faturamento-via-excel-3.png "Importar regras de faturamento via Excel - 3")

Em caso de erro, a planilha poderá se corrigida e importada, quantas vezes necessário. Na re-importação o sistema altera a regra previamente criada, encontrando-a pelo nome do contrato e título informados na planilha.