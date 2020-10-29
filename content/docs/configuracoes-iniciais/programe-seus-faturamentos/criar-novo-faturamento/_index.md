---
title: Criar novo faturamento
layout: blog
weight: 1
---
Para criar um novo faturamento, selecione um contrato previamente criado e clique em “Criar Novo Faturamento”. 

Caso ainda não tenha criado o contrato, consulte o tópico [Criar novo contrato](/docs/configuracoes-iniciais/cadastre-seus-contratos/criar-novo-contrato/).

![No terceiro tópico (Faturamentos) do contrato, uma seta destaca o botão "Criar Novo Faturamento".](/images/uploads/criar-novo-faturamento-1.png "Criar novo faturamento - 1")

Uma nova tela irá se abrir. Vá até a seção “Serviços” e adicione os serviços que serão cobrados neste faturamento, clicando em Adicionar. É possível adicionar mais de um serviço, ok? Para cada um deles informe uma descrição, a quantidade e o valor unitário. 

O valor total do faturamento será a soma do valor de cada serviço.

Para criar previamente os serviços, consulte o tópico [Criar novo serviço](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.4lfr4d4xsbck).

![Na seção "Serviços" tem um botão destacado, botão "Adicionar".](/images/uploads/criar-novo-faturamento-2.png "Criar novo faturamento - 2")

Em “Clientes”, informe o cliente a ser faturado. Por padrão o Billimatic sugere o mesmo cliente do contrato, mas você pode alterar esse dado caso necessário. É o caso, por exemplo, de contratos firmados com a matriz onde as filiais são faturadas.

![Exemplo de cadastro de cliente.](/images/uploads/criar-novo-faturamento-3.png "Criar novo faturamento - 3")

Na seção “Faturamento”, informe:

* Previsão - Data prevista para o faturamento.
* Valor a receber
* Tipo de faturamento - Para emitir a NFS-e, boleto de cobrança, transação de cartão de crédito e notificações de forma automática na data prevista, escolha a opção de Faturamento Automático. Caso deseje que o sistema aguarde o comando do usuário para tomar as ações descritas, escolha a opção de Faturamento Manual.
* Descrição - Descreve o que está sendo faturado. É a descrição que aparece na fatura enviada aos seus clientes.
* Régua de cobrança - Selecione qual régua de notificação irá realizar as notificações a respeito deste faturamento. Saiba mais no tópico [Configurar réguas de cobrança](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.n5jqgcye9bui).
* Mês de competência - É o mês em que ocorreu o evento que gerou o faturamento.

![Exemplo de formulário de "Faturamento".](/images/uploads/criar-novo-faturamento-4.png "Criar novo faturamento - 4")

Na seção “Vencimentos” indique a data de vencimento das cobranças. Corresponde à data de vencimento do boleto.

Normalmente um faturamento possui uma única data de vencimento. Mas se o faturamento for parcelado, então cada parcela terá a sua própria data de vencimento.

O % de valor bruto diz respeito a quanto, do valor total do faturamento, corresponde o valor cobrado em cada vencimento. Por exemplo, caso o faturamento seja parcelado em 2 vezes, o percentual do valor bruto será de 50% para cada vencimento.

![Exemplo de forumlário de "Vencimentos".](/images/uploads/criar-novo-faturamento-5.png "Criar novo faturamento - 5")

Na seção “Nota Fiscal”, informe:

* Número da nota
* Emissão da Nota
* Código de verificação
* Modelo de NFS-e (Emites) - Selecione qual modelo de NFS-e será utilizado neste faturamento. Caso ainda não tenha definido seus modelos, consulte o tópico [Configurar notas fiscais](https://docs.google.com/document/d/1psChi3xUnRTthgMP8Ibs6UMBDaQgmrWYey5ikBIobiY/edit#heading=h.sbh8t7q6hime).
* Quando deseja emitir a NFS-e: no dia do faturamento ou dias depois do recebimento. A vantagem de atrelá-la ao recebimento é não ter emitido a nota, em caso de inadimplência e posterior perda do faturamento. Esta é uma opção para uso no faturamento automático.
* Corpo da NFS-e - Insira aqui a descrição da nota fiscal. Note que você pode utilizar tags de substituição com os dados do faturamento. Essas tags serão substituídas pelos valores correspondentes no momento da emissão da nota. No exemplo abaixo a tag será substituída pela descrição do faturamento. A lista completa das tags disponíveis podem ser consultadas na própria tela.

![Exemplo de formulário de "Nota Fiscal".](/images/uploads/criar-novo-faturamento-6.png "Criar novo faturamento - 6")

Na seção “Cobrança”, informe:

* Forma de pagamento: boleto, cartão de crédito ou transferência
* Configuração de Cobrança (Cobrato) - Escolha qual configuração de cobrança será utilizada neste faturamento. Caso a forma de pagamento escolhida for boleto, a configuração de cobrança irá definir o banco e a respectiva conta de cobrança. Para o caso de pagamento feito por cartão de crédito, define a conta da Cielo. 
* Modelo de Cobrança (Cobrato) - Para o caso de boletos, define a política de multa e juros, para cálculo de boletos vencidos. 

![Exemplo de formulário de "Cobrança".](/images/uploads/criar-novo-faturamento-7.png "Criar novo faturamento - 7")

Na seção “Financeiro”, você irá incluir as informações necessárias para associar o vencimento a um recebível no Myfinance. Esta seção aparece somente para quem tem integração com o sistema Myfinance. Saiba mais em **Integrações**.

* Categoria - O recebível associado é categorizado conforme a categoria selecionada.
* Centro de Receita - O recebível associado é apropriado ao centro de receita selecionado.
* Conta de Recebível - O recebível associado usa regras definidas na conta de recebível selecionada.

![Exemplo de formulário de "Financeiro".](/images/uploads/criar-novo-faturamento-8.png "Criar novo faturamento - 8")

Na seção “Observações” podem ser informadas quaisquer informações relevantes, durante o ciclo de vida do faturamento.

![Exemplo de formulário de "Observações".](/images/uploads/criar-novo-faturamento-9.png "Criar novo faturamento - 9")

Finalmente, em Documentos podem ser anexados quaisquer arquivos relevantes, durante o ciclo de vida do faturamento.

A nota fiscal, fatura e boleto já encontram-se associados ao faturamento, não sendo necessária sua adição.

![Na seção "Documentos", o botão "Adicionar" está destacado por uma seta.](/images/uploads/criar-novo-faturamento-10.png "Criar novo faturamento - 10")