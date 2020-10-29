---
title: Criar nova regra de faturamento
layout: blog
weight: 3
---
As regras de faturamento são um dos grandes diferenciais do Billimatic. São um grande facilitador na hora de criar os faturamentos, pois através dela é possível criar faturamentos recorrentes, em diferentes periodicidades, ou faturamentos que se repetem até um prazo delimitado.

Ao criar uma regra, todos os faturamentos são gerados automaticamente, dentro dos critérios definidos na mesma.

Para faturamentos recorrentes, também permite automatizar reajustes de valor, a partir de índices econômicos, como IGP-M, IPCA, etc.

Neste tópico vamos aprender como criar manualmente uma regra avulsa, mas você pode criar várias regras ao mesmo tempo através de uma planilha de Excel. Para saber mais, consulte o tópico [Importar regras de faturamento via Excel](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.h20rgwk94i4r).

Para criar uma nova regra de faturamento da forma convencional, selecione um contrato previamente criado e clique em “Criar Nova Regra”. (Caso ainda não tenha criado o contrato, consulte o tópico [Criar novo contrato](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.6vsmkox48u0q)).

Na seção “Informações Gerais”, identifique a regra com um título.

Dica! Além das regras de faturamento, utilize também os modelos de faturamento para preencher automaticamente dados da regra. Caso ainda não tenha criado um modelo de faturamento, consulte o tópico [Criar modelo de faturamento](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.bm6v1a42ucr3).

![Exemplo de formulário de "Informações Gerais".](/images/uploads/criar-nova-regra-de-faturamento-1.png "Criar nova regra de faturamento - 1")

Em “Clientes”, informe o cliente a ser faturado. Por padrão o Billimatic sugere o mesmo cliente do contrato, mas você pode alterar esse dado caso necessário. É o caso, por exemplo, de contratos firmados com a matriz onde as filiais são faturadas.

![Exemplo de formulário de "Cliente".](/images/uploads/criar-novo-faturamento-3.png "Criar nova regra de faturamento - 2")

Na seção “Serviços”, adicione os serviços que serão cobrados neste faturamento, clicando no botão “Adicionar”. É possível adicionar mais de um serviço, ok? Para cada um deles informe uma descrição, a quantidade e o valor unitário. O valor total do faturamento será a soma do valor de cada serviço.

Caso ainda não tenha criado os serviços, consulte o tópico [Criar novo serviço](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.4lfr4d4xsbck).

![Na seção "Serviços", o botão "Adicionar" está destacado por uma seta.](/images/uploads/criar-novo-faturamento-2.png "Criar nova regra de faturamento - 3")

Preencha a regra da periodicidade do Faturamento, informando a data inicial, a periodicidade e a data final da cobrança (deixe em branco caso seja um faturamento recorrente).

Por exemplo:

1. Criar o primeiro faturamento em 01/07/2020, repetindo-o mensalmente, até dia 01/10/2020: neste caso, no dia 01 dos meses de Julho, Agosto, Setembro e Outubro, ocorrerá o faturamento de acordo com as regras estabelecidas.
2. Criar o primeiro faturamento em 01/07/2020, repetindo-o anualmente, até dia 01/07/2025: aqui, o faturamento será acionado no dia 01/07 de cada ano, até 2025.

Continue preenchendo os dados da regra:

* Tipo de Faturamento: Automático ou manual

Para emitir a NFS-e, boleto de cobrança, transação de cartão de crédito e notificações de forma automática na data prevista, escolha a opção de Faturamento Automático. Caso deseje que o sistema aguarde o comando do usuário para tomar as ações descritas, escolha a opção de Faturamento Manual.

Para o faturamento automático, obrigatoriamente deve ser selecionado o modelo de notificação.

* Descrição - Descreve o que está sendo faturado. É a descrição que aparece na fatura enviada aos seus clientes.
* Régua de notificação - Selecione qual régua de notificação irá realizar as notificações a respeito deste faturamento. Saiba mais no tópico [Configurar réguas de cobrança](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.n5jqgcye9bui).
* Competência - permite definir a competência do faturamento no mesmo mês do faturamento, ou ao mês anterior ao faturamento.

![Exemplo de formulário de "Faturamento".](/images/uploads/criar-novo-faturamento-4.png "Criar nova regra de faturamento - 4")

Na seção “Vencimento” você irá configurar as regras para o cálculo da data de vencimento de cada faturamento. É só selecionar qual das opções se adequa melhor à sua necessidade e preencher as lacunas.

Por exemplo, se selecionada a opção “No próximo dia 10 após a data do faturamento”, um faturamento com previsão em 01/08/2020 terá data de vencimento calculada em 10/08/2020.

Caso queira gerar parcelas, selecione a opção “Dividir em n parcelas iguais” e indique o número de parcelas a serem cobradas mensalmente a partir da data de vencimento escolhida anteriormente.

![Exemplo de formulário de "Informações de Vencimento".](/images/uploads/criar-nova-regra-de-faturamento-2.png "Criar nova regra de faturamento - 5")

Na seção “Configurações de reajuste automático” o Billimatic praticamente salva sua vida (e tempo) de atualizar manualmente os índices de reajuste. Imagina ter que fazer isso a cada reajuste, o trabalho que dá. Bom, agora fazemos isso pra você.

Vamos pegar de exemplo um contrato recorrente, firmado em 01/07/2020, reajustado anualmente com base no IGP-M.

Para este caso, devem ser informados:

* Primeiro reajuste - Data do primeiro reajuste. No caso do exemplo a data do primeiro reajuste ocorrerá no próximo ano, em 01/07/2021.
* Periodicidade do reajuste - Número de meses em que ocorre o reajuste. No exemplo anterior são 12 (meses).
* Índice - O índice econômico usado no reajustes. No exemplo anterior: IGP-M.
* Notificação (dias) - Aqui você indica quantos dias antes a sua equipe administrativa, e opcionalmente o seu cliente, será avisado do reajuste. No exemplo anterior, se para o campo “Notificação (dias)” for informado 31 dias, a notificação será enviada um mês antes do dia do reajuste. É sempre uma boa prática deixar todo mundo ciente dos reajustes, principalmente o seu cliente.
* Selecione a opção “Notificar cliente” permite que seu cliente seja notificado por e-mail para notificá-lo por e-mail sobre o reajuste.
* A opção “Permitir reajuste negativo” zera o reajuste, caso a alíquota acumulada no período seja negativa, ou seja, caso o reajuste diminua o valor do contrato.

  ![](/images/uploads/image42.png)

Caso o seu faturamento tenha mais de um serviço selecionado, é possível reajustar cada um deles individualmente, em datas e usando índices distintos. Para isso, adicione configurações para cada serviço clicando no botão “Adicionar” e selecione o serviço específico.

Na seção “Nota Fiscal”, informe:

* Modelo de NFS-e (Emites) - Selecione qual modelo de NFS-e será utilizado neste faturamento. Caso ainda não tenha definido seus modelos, consulte o tópico [Configurar notas fiscais](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.sbh8t7q6hime).
* Escolha quando deseja emitir a NFS-e: no dia do faturamento ou dias depois do recebimento. A vantagem de atrelá-la ao recebimento é não ter emitido a nota, em caso de inadimplência e posterior perda do faturamento. Esta é uma opção para uso no faturamento automático.
* Corpo da NFS-e - Insira aqui a descrição da nota fiscal. Note que você pode utilizar tags de substituição com os dados do faturamento. Essas tags serão substituídas pelos valores correspondentes no momento da emissão da nota. No exemplo abaixo a tag será substituída pela descrição do faturamento. A lista completa das tags disponíveis podem ser consultadas na própria tela.

Na seção “Cobrança”, informe:

* Forma de pagamento: Boleto, cartão de crédito ou transferência
* Configuração de Cobrança (Cobrato) - Escolha qual configuração de cobrança será utilizada neste faturamento. Caso a forma de pagamento escolhida for boleto, a configuração de cobrança irá definir o banco e a respectiva conta de cobrança. Para o caso de pagamento feito por cartão de crédito, define a conta da Cielo. 
* Modelo de Cobrança (Cobrato) - Para o caso de boletos, define a política de multa e juros, para cálculo de boletos vencidos. 

Na seção “Financeiro”, você irá incluir as informações necessárias para associar o vencimento a um recebível no Myfinance. Esta seção aparece somente para quem tem integração com o sistema Myfinance. Saiba mais em Integrações.

* Categoria - O recebível associado é categorizado conforme a categoria selecionada.
* Centro de Receita - O recebível associado é apropriado ao centro de receita selecionado.
* Conta de Recebível - O recebível associado usa regras definidas na conta de recebível selecionada.