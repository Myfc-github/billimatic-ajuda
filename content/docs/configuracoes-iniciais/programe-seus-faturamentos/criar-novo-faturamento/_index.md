---
title: Criar novo faturamento
layout: blog
weight: 1
---
Para criar um novo faturamento, selecione um contrato previamente criado e clique em “Criar Novo Faturamento”. (Caso ainda não tenha criado o contrato, consulte o tópico [Criar novo contrato](/docs/configuracoes-iniciais/cadastre-seus-contratos/criar-novo-contrato/)).

![No terceiro tópico (Faturamentos) do contrato, uma seta destaca o botão "Criar Novo Faturamento".](/images/uploads/criar-novo-faturamento-1.png "Criar novo faturamento - 1")

Na seção “Serviços”, adicione os serviços que serão faturados, clicando no botão “Adicionar”. Para cada serviço, informe uma descrição, quantidade e valor unitário. O valor total do faturamento será a soma do valor de cada serviço.

Nota, caso ainda não tenha criado os serviços, consulte o tópico [Criar novo serviço](/docs/configuracoes-iniciais/configure-sua-organizacao/criar-novo-serviço/).

![Na seção "Serviços" tem um botão destacado, botão "Adicionar".](/images/uploads/criar-novo-faturamento-2.png "Criar novo faturamento - 2")

Na seção “Clientes”, informe o cliente a ser faturado. Por padrão o Billimatic sugere o mesmo cliente do contrato. Porém ele permite que um cliente diferente do contrato seja faturado. É o caso, por exemplo, de contratos firmados com a matriz, porém com suas filiais faturadas.

![Exemplo de cadastro de cliente.](/images/uploads/criar-novo-faturamento-3.png "Criar novo faturamento - 3")

Na seção “Faturamento”, informe:

* Previsão - Data prevista para o faturamento.
* Tipo de Faturamento - O faturamento automático é disparado automaticamente na data prevista, emitindo a NFS-e, boleto de cobrança ou transação de cartão de crédito, e notificando os clientes. Já o faturamento manual aguarda o usuário comandar todas as ações descritas no faturamento automático.

Para o faturamento automático, obrigatoriamente deve ser selecionado o modelo de notificação.

* Descrição - Descreve o que está sendo faturado. É a descrição que aparece na fatura enviada aos seus clientes.
* Régua de cobrança - A régua de cobrança define uma política de notificações enviadas para os clientes, ao longo do ciclo de vida do faturamento. Saiba mais no tópico [Configurar réguas de cobrança](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit?ts=5f4547ec#heading=h.n5jqgcye9bui).
* Mês de competência - Refere-se ao mês de competência da prestação do serviço.

![Exemplo de formulário de "Faturamento".](/images/uploads/criar-novo-faturamento-4.png "Criar novo faturamento - 4")

Na seção “Vencimentos” devem ser informados as datas de vencimento das cobranças. A data de vencimento corresponde à data limite para o pagamento pelo seu cliente. Corresponde à data de vencimento do boleto.

Normalmente um faturamento possui uma única data de vencimento. Múltiplas datas de vencimento indicam o parcelamento do faturamento em múltiplos boletos.

Para cada vencimento, informe a data e o percentual do valor bruto do faturamento. Por exemplo, caso o faturamento seja parcelado em 2 vezes, o percentual do valor bruto será de 50% para cada vencimento.

![Exemplo de forumlário de "Vencimentos".](/images/uploads/criar-novo-faturamento-5.png "Criar novo faturamento - 5")

Na seção “Nota Fiscal”, informe:

* Modelo de NFS-e (Emites) - Modelo de NFS-e configurado no Emites. O modelo define os parâmetros da nota fiscal, como código do serviço na prefeitura, alíquota de ISS, retenção de impostos, impostos aproximados. Caso ainda não tenha definido seus modelos, consulte o tópico [Configurar notas fiscais](/docs/notas-fiscais/configure-suas-notas-fiscais/).
* Emitir nota fiscal no dia do faturamento ou após n dias úteis do recebimento. Esta é uma opção para uso no faturamento automático. A nota pode ser emitida junto com a fatura, ou sua emissão pode ser atrelada ao recebimento. A vantagem de atrelá-la ao recebimento é não ter emitido a nota, em caso de inadimplência e posterior perda do faturamento.
* Corpo da NFS-e - Conteúdo do corpo da NFS-e. No corpo é possível utilizar tags de substituição com os dados do faturamento. No exemplo da imagem abaixo a tag $DESCRICAO será substituída pela descrição do faturamento, no momento da emissão da nota. A lista completa das tags disponíveis podem ser consultadas na própria tela.

![Exemplo de formulário de "Nota Fiscal".](/images/uploads/criar-novo-faturamento-6.png "Criar novo faturamento - 6")

Na seção “Cobrança”, informe:

* Forma de pagamento - Boleto bancário, Cartão de crédito ou Transferência bancária.
* Configuração de Cobrança (Cobrato) - Para o caso de boletos, define o banco e a respectiva conta de cobrança. Para o caso de cartão de crédito, define a conta da Cielo. Caso ainda não tenha configurado as cobranças, consulte o tópico [Configurar cobranças](/docs/integracoes/configurar-cobrancas/).
* Modelo de Cobrança (Cobrato) - Para o caso de boletos, define a política de multa e juros, para cálculo de boletos vencidos.

![Exemplo de formulário de "Cobrança".](/images/uploads/criar-novo-faturamento-7.png "Criar novo faturamento - 7")

Na seção “Financeiro”, informe: (Somente para integração com o Myfinance)

Cada vencimento será associado a um recebível no Myfinance.

* Categoria - O recebível associado é categorizado conforme a categoria selecionada.
* Centro de Receita - O recebível associado é apropriado ao centro de receita selecionado.
* Conta de Recebível - O recebível associado usa regras definidas na conta de recebível selecionada.

![Exemplo de formulário de "Financeiro".](/images/uploads/criar-novo-faturamento-8.png "Criar novo faturamento - 8")

Na seção “Observações” podem ser informadas quaisquer informações relevantes, durante o ciclo de vida do faturamento.

![Exemplo de formulário de "Observações".](/images/uploads/criar-novo-faturamento-9.png "Criar novo faturamento - 9")

Na seção “Documentos” podem ser anexados quaisquer arquivos relevantes, durante o ciclo de vida do faturamento.

Nota: A nota fiscal, fatura e boleto já encontram-se associados ao faturamento, não sendo necessária sua adição.

![Na seção "Documentos", o botão "Adicionar" está destacado por uma seta.](/images/uploads/criar-novo-faturamento-10.png "Criar novo faturamento - 10")