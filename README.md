# Nanu Som · Orçamentos

Sistema de orçamentos que roda direto no navegador, sem servidor e sem banco de dados. Esta versão já traz os **27 orçamentos** que você enviou em PDF.

## Arquivos para enviar ao GitHub

| Arquivo | O que é |
|---|---|
| `index.html` | O sistema. |
| `dados-iniciais.js` | Os orçamentos e clientes antigos (carregados na primeira abertura). |
| `README.md` | Este guia (opcional). |

Os dois primeiros são obrigatórios e precisam ficar **na mesma pasta**.

## Como publicar (você já tem o repositório `nanu-som`)

1. Entre em https://github.com e abra o repositório `nanu-som`.
2. Clique em **Add file → Upload files**.
3. Arraste `index.html` e `dados-iniciais.js` para a tela. (Se o GitHub avisar que já existem arquivos com esses nomes, tudo bem: eles serão substituídos.)
4. Clique em **Commit changes**.
5. Espere 1 a 2 minutos. Abra o endereço do site (`https://SEU-USUARIO.github.io/nanu-som/`) e use **Ctrl + F5** (no celular, feche e abra o navegador) para carregar a versão nova.

Se você ainda não tem o repositório: **+ → New repository**, nome `nanu-som`, **Public**; envie os arquivos como acima; depois **Settings → Pages → Source: Deploy from a branch → Branch: main, pasta / (root) → Save**.

## O que acontece na primeira abertura

- O sistema lê o `dados-iniciais.js` e **junta** os orçamentos antigos com o que já existe no navegador. **Nada é apagado nem sobrescrito.** Só entra o que ainda não existe.
- Antes de juntar, ele guarda uma cópia dos dados atuais no próprio navegador. Se der qualquer erro, seus dados ficam exatamente como estavam.
- Aparece um aviso "Importação inicial: N orçamento(s) adicionado(s)". O resumo fica em **Configurações → Orçamentos importados**.
- Isso acontece **uma única vez por navegador**. Se você apagar um orçamento depois, ele não volta.
- Onde já há orçamentos (o notebook em que você os criou), os que já existem **não são alterados**. Os orçamentos do Lipeh (nº 0007) e do Moraes (nº 0011), que foram impressos em versões diferentes, são comparados pelo conteúdo: o que for diferente do que já está no sistema entra como **orçamento novo, com número novo**. Veja o `RELATORIO-IMPORTACAO.md`.

## Entrada e saldo restante (novo)

Na tela de criar/editar orçamento, o campo **Entrada solicitada (R$)** é opcional. Ao preencher, o sistema calcula o **saldo restante** (total − entrada) na hora. No orçamento mostrado ao cliente, na impressão e no PDF aparecem as linhas **Entrada** e **Saldo restante**, mas só quando há entrada. A entrada não pode ser maior que o total. Orçamentos antigos não têm entrada.

## Limites que você precisa conhecer

- **Os dados ficam só no navegador de cada aparelho.** O notebook e o celular **não** se sincronizam: o celular recebe os mesmos 27 orçamentos antigos na primeira abertura, mas o que você criar depois fica só onde foi criado. Para levar de um aparelho a outro, use **Configurações → Exportar backup** e **Importar backup** (a importação do backup **substitui** os dados do aparelho; confirme antes).
- Limpar os dados do navegador apaga os orçamentos que não estiverem em backup. Exporte um backup de vez em quando.
- **O login só confere no navegador e não protege dados.** Com repositório público, qualquer pessoa pode ver o código do site.

## ⚠️ Privacidade: leia antes de publicar

O arquivo `dados-iniciais.js` contém **nomes e telefones dos seus clientes**, junto com os orçamentos. No GitHub Pages gratuito o repositório é **público**: qualquer pessoa que souber o endereço do arquivo consegue ler esses dados, mesmo sem entrar no sistema.

Opções para evitar:
- Usar um repositório **privado** com GitHub Pages (disponível apenas em planos pagos do GitHub); ou
- Não publicar o `dados-iniciais.js` e, em vez disso, levar os orçamentos de cada aparelho por **backup** (arquivo guardado só com você).

Se preferir não expor os dados, me avise que eu preparo essa versão.
