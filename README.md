## Desenvolvimento

**Hugo**

Para levantar o projeto localmente, basta executar no console:

> hugo serve

Feito isto, basta acessar no navegador através de *http://localhost:1313/*

**Netlify CMS - Admin**

Para acessar o admin do Netlify CMS, basta inserir o diretorio */admin/* no navegador. No momento, só convidados através do Netlify Identity podem se cadastrar e acessar o admin com login e senha.
As páginas criadas através do admin são enviadas para o branch main através de commits automaticamente. Para criar páginas no admin *localmente*, é preciso executar no console (abra uma janela apenas para isso) uma Beta Feature do Netlify CMS:

> npx netlify-cms-proxy-server

Agora, ao invés de logar no admin com a autenticação, haverá um botão "Entrar" e o conteúdo criado será gerenciado no próprio branch.

**Gulp**

É possível escrever os estilos em Sass no projeto através do gulp. Para compilar os arquivos Sass para CSS, basta executar no console:

> gulp sass

Para manter o gulp ativo no console compilando o CSS a cada nova alteração no Sass, existe a opção *gulp watch*:

> gulp watch

Estes comandos irão compilar os aquivos dentro de assets/sass e sobrescrevê-los dentro de assets/css.
