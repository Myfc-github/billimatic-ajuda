---
title: Criar nova regra de faturamento
layout: blog
weight: 3
---
A regra de faturamento é um facilitador para que você crie seus faturamentos. Através dela é possível criar faturamentos recorrentes, em diferentes periodicidades, ou faturamentos que se repetem até um prazo delimitado.

Ao criar uma regra, todos os faturamentos são gerados automaticamente, dentro dos critérios definidos na mesma.

Para faturamentos recorrentes, também permite automatizar reajustes de valor, a partir de índices econômicos, como IGP-M, IPCA, etc.

Para criar uma nova regra de faturamento, selecione um contrato previamente criado e clique em “Criar Nova Regra”. (Caso ainda não tenha criado o contrato, consulte o tópico [Criar novo contrato](/docs/configuracoes-iniciais/cadastre-seus-contratos/criar-novo-contrato/)).

Alternativamente as regras podem ser criadas através de planilha Excel. Para saber mais, consulte o tópico [Importar regras de faturamento via Excel](/docs/configuracoes-iniciais/programe-seus-faturamentos/importar-regras-de-faturamento-via-excel/).

Na seção “Informações Gerais”, identifique a regra com um título.

Opcionalmente é possível selecionar um modelo de faturamento, previamente cadastrado, para preencher automaticamente dados da regra. Caso ainda não tenha criado um modelo de faturamento, consulte o tópico [Criar modelo de faturamento](/docs/configuracoes-iniciais/programe-seus-faturamentos/criar-modelo-de-faturamento/).

![Exemplo de formulário de "Informações Gerais".](/images/uploads/criar-nova-regra-de-faturamento-1.png "Criar nova regra de faturamento - 1")

Na seção “Cliente”, informe o cliente a ser faturado. Por padrão o Billimatic sugere o mesmo cliente do contrato. Porém ele permite que um cliente diferente do contrato seja faturado. É o caso, por exemplo, de contratos firmados com a matriz, porém com suas filiais faturadas.

![Exemplo de formulário de "Cliente".](/images/uploads/criar-novo-faturamento-3.png "Criar nova regra de faturamento - 2")

Na seção “Serviços”, adicione os serviços que serão faturados, clicando no botão “Adicionar”. Para cada serviço, informe uma descrição, quantidade e valor unitário. O valor total do faturamento será a soma do valor de cada serviço.

Nota, caso ainda não tenha criado os serviços, consulte o tópico [Criar novo serviço](/docs/configuracoes-iniciais/configure-sua-organizacao/criar-novo-serviço/).

![Na seção "Serviços", o botão "Adicionar" está destacado por uma seta.](/images/uploads/criar-novo-faturamento-2.png "Criar nova regra de faturamento - 3")

Na seção “Faturamento”, informe:

* Criar o primeiro faturamento em - Esta é a data em que será criado o primeiro faturamento, e a partir deste, serão criados os posteriores.
* repetindo-o - periodicidade de repetição dos faturamentos. Por exemplo, caso seja definido o primeiro faturamento no dia 01/07/2020 e periodicidade mensal, serão criados faturamentos em 01/07/2020, 01/08/2020, 01/09/2020, e assim por diante.
* até o dia - data limite até a qual serão criados os faturamentos. Se desejar que o faturamento seja recorrente, a data deve ser deixada em branco.
* Tipo de Faturamento - O faturamento automático é disparado automaticamente na data prevista, emitindo a NFS-e, boleto de cobrança ou transação de cartão de crédito, e notificando os clientes. Já o faturamento manual aguarda o usuário comandar todas as ações descritas no faturamento automático.

Para o faturamento automático, obrigatoriamente deve ser selecionado o modelo de notificação.

* Descrição - Descreve o que está sendo faturado. É a descrição que aparece na fatura enviada aos seus clientes.
* Régua de cobrança - A régua de cobrança define uma política de notificações enviadas para os clientes, ao longo do ciclo de vida do faturamento. Saiba mais no tópico [Configurar réguas de cobrança](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit?ts=5f4547ec#heading=h.n5jqgcye9bui).
* Competência - permite definir a competência do faturamento no mesmo mês do faturamento, ou ao mês anterior ao faturamento.

![Exemplo de formulário de "Faturamento".](/images/uploads/criar-novo-faturamento-4.png "Criar nova regra de faturamento - 4")

Na seção “Vencimento”, configure as regras para o cálculo da data de vencimento de cada faturamento.

Por exemplo, se selecionada a opção “No próximo dia 10 após a data do faturamento”, um faturamento com previsão em 01/08/2020 terá data de vencimento calculada em 10/08/2020.

A opção “Dividir em n parcelas iguais” parcela o faturamento igualmente no número informado. No exemplo anterior, caso fosse selecionada a opção “Dividir em 2 parcelas iguais”, seriam criados dois vencimentos, um em 10/08/2020 e outro em 10/09/2020.

![Exemplo de formulário de "Informações de Vencimento".](/images/uploads/criar-nova-regra-de-faturamento-2.png "Criar nova regra de faturamento - 5")

Na seção “Configurações de reajuste automático” pode ser definida regra para que os faturamentos sejam reajustados automaticamente, ao longo do tempo,

Por exemplo, um contrato recorrente, firmado em 01/07/2020, reajustado anualmente com base no IGP-M.

Para este caso, devem ser informados:

* Primeiro reajuste - Data do primeiro reajuste. No exemplo anterior, a data do primeiro reajuste ocorrerá no próximo ano, em 01/07/2021.
* Periodicidade do reajuste - Número de meses em que ocorre o reajuste. No exemplo anterior, o valor é de 12 (meses).
* Índice - O índice econômico usado no reajustes. No exemplo anterior: IGP-M.
* Notificação (dias) - Número de dias em que sua equipe administrativa, e opcionalmente o seu cliente, será avisado do reajuste. No exemplo anterior, se para o campo “Notificação” (dias) for informado 31 dias, será enviado uma notificação um mês antes do dia do reajuste.
* A opção “Notificar cliente” permite que seu cliente seja notificado por e-mail, do aviso que o contrato será reajustado, e do reajuste em si.
* A opção “Permitir reajuste negativo” zera o reajuste, caso a alíquota acumulada no período seja negativa, ou seja, caso o reajuste diminua o valor do contrato.

  ![Exemplo de formulário de "Configurações de Reajuste Automático".](/images/uploads/criar-nova-regra-de-faturamento-3.png "Criar nova regra de faturamento - 6")

  * Para regras com mais de um serviço faturado, é possível reajustar determinados serviços individualmente, em datas e usando índices distintos. Para isso, adicione configurações clicando no botão “Adicionar” e selecione o serviço específico.

  ![Exemplo de formulário de "Configurações de Reajuste Automático".](/images/uploads/criar-nova-regra-de-faturamento-3.png "Criar nova regra de faturamento - 7")

  Na seção “Nota Fiscal”, informe:

  * Modelo de NFS-e (Emites) - Modelo de NFS-e configurado no Emites. O modelo define os parâmetros da nota fiscal, como código do serviço na prefeitura, alíquota de ISS, retenção de impostos, impostos aproximados. Caso ainda não tenha definido seus modelos, consulte o tópico [Configurar notas fiscais](/docs/notas-fiscais/configure-suas-notas-fiscais/).
  * Emitir nota fiscal no dia do faturamento ou após n dias úteis do recebimento. Esta é uma opção para uso no faturamento automático. A nota pode ser emitida junto com a fatura, ou sua emissão pode ser atrelada ao recebimento. A vantagem de atrelá-la ao recebimento é não ter emitido a nota, em caso de inadimplência e posterior perda do faturamento.
  * Corpo da NFS-e - Conteúdo do corpo da NFS-e. No corpo é possível utilizar tags de substituição com os dados do faturamento. No exemplo da imagem abaixo a tag $DESCRICAO será substituída pela descrição do faturamento, no momento da emissão da nota. A lista completa das tags disponíveis podem ser consultadas na própria tela.

  ![Exemplo de formulário de "Nota Fiscal".](/images/uploads/criar-novo-faturamento-6.png "Criar nova regra de faturamento - 8")

  Na seção “Cobrança”, informe:

  * Forma de pagamento - Boleto bancário, Cartão de crédito ou Transferência bancária.
  * Configuração de Cobrança (Cobrato) - Para o caso de boletos, define o banco e a respectiva conta de cobrança. Para o caso de cartão de crédito, define a conta da Cielo. Caso ainda não tenha configurado as cobranças, consulte o tópico [Configurar cobranças](/docs/integracoes/configurar-cobrancas/).
  * Modelo de Cobrança (Cobrato) - Para o caso de boletos, define a política de multa e juros, para cálculo de boletos vencidos.

    ![Exemplo de formulário de "Cobrança".](/images/uploads/criar-novo-faturamento-7.png "Criar nova regra de faturamento - 8")

    Na seção “Financeiro”, informe: (Somente para integração com o Myfinance)

    Cada vencimento será associado a um recebível no Myfinance.

    * Categoria - O recebível associado é categorizado conforme a categoria selecionada.
    * Centro de Receita - O recebível associado é apropriado ao centro de receita selecionado.
    * Conta de Recebível - O recebível associado usa regras definidas na conta de recebível selecionada.

      ![Exemplo de formulário de "Financeiro".](/images/uploads/criar-novo-faturamento-8.png "Criar nova regra de faturamento - 8")