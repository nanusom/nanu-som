# NANU SOM · Orçamentos — atualização de 22/10 (documento do cliente)

Arquivos (todos na raiz do repositório do GitHub Pages):

| Arquivo | O que é |
|---|---|
| `index.html` | O sistema completo (substitui o atual). |
| `dados-iniciais.js` | Os 27 orçamentos importados dos PDFs (substitui o atual). |
| `README.md` | Este guia (opcional no repositório). |
| `RELATORIO-IMPORTACAO.md` | Relatório da importação dos 27 PDFs (opcional). |

## O que mudou no orçamento que o cliente recebe
1. **OBSERVAÇÕES IMPORTANTES**: bloco próprio, com borda azul, fundo claro e texto de 16,5 px, logo abaixo dos dados do cliente e **antes dos itens**. O texto aparece completo e o bloco não é cortado ao meio na impressão/PDF.
2. **Valores com nova hierarquia** (quando há entrada):
   - *Valor total do orçamento* (legível, sem destaque máximo);
   - *Entrada paga* + "Valor já recebido" (ou *Entrada solicitada* + "Pendente: ainda não recebida");
   - **Falta pagar / Saldo restante**: o maior destaque (barra preta, letra grande).
   Exemplo: total R$ 500,00 · entrada paga R$ 100,26 · falta pagar R$ 399,74.
3. **Situação da entrada**: novo campo no editor, "Pendente" (padrão) ou "Paga". A entrada só é tratada como recebida quando marcada como **Paga**.
4. Sem entrada: o documento continua com a barra "Total" de sempre e uma linha pequena "Entrada: não solicitada".

5. **Impressão/PDF**: o bloco de totais, as observações e o rodapé não são cortados ao meio. Em orçamentos com muitos itens, os totais podem ir para a página 2, juntos com as condições e o rodapé.

Nada mais foi alterado: clientes, produtos, medidas das caixas, itens, histórico, impressão, PDF e WhatsApp seguem iguais. A litragem continua oculta do cliente.

## ⚠️ Única mudança que mexe em dados já existentes
Antes, o saldo era sempre *total − entrada*. Agora o saldo é *total − pagamentos já recebidos*. Por isso:
- **Orçamentos antigos que tinham valor de entrada, mas nenhum status, passam a aparecer como "Entrada solicitada" (pendente)** e o "Falta pagar" será o total. Nenhum valor é alterado nem apagado.
- Para os que já foram pagos: abra o orçamento → **Editar** → "Situação da entrada" = **Paga** → Salvar.
- Orçamentos sem entrada não mudam.

## Como atualizar sem perder nada
Os orçamentos ficam **dentro do navegador** (não nos arquivos do GitHub). Substituir os arquivos não apaga os dados, mas faça o backup mesmo assim:
1. No sistema atual (nos aparelhos que têm dados): **Configurações → Exportar backup** e guarde o arquivo `.json`.
2. No GitHub: repositório → **Add file → Upload files** → arraste `index.html` e `dados-iniciais.js` (substituem os antigos) → **Commit changes**.
3. Espere 1–2 minutos e abra `https://nanusom.github.io/nanu-som/` (atualize com Ctrl+F5; no celular, recarregue a página).
4. Confira se os orçamentos continuam lá. Se algo parecer errado, use **Configurações → Importar backup** com o arquivo do passo 1.
5. Marque como **Paga** as entradas já recebidas (ver aviso acima).

A importação inicial dos 27 PDFs é **aditiva**: só acrescenta o que faltar, não sobrescreve, não repete números e faz uma cópia de segurança automática no navegador antes de mexer. Detalhes em `RELATORIO-IMPORTACAO.md` da entrega anterior.

## Avisos honestos
- O login (nanosom / ns@24) roda no próprio navegador: **não é segurança de verdade**.
- Repositório gratuito do GitHub Pages é **público**: `dados-iniciais.js` expõe nomes e telefones de clientes. Para evitar, remova esse arquivo depois da importação (os dados já ficam no navegador) e importe por backup nos outros aparelhos.
- Os dados são por navegador/aparelho: o celular não vê o que está no notebook sem Exportar/Importar backup.
- O azul foi usado nas observações e na entrada; o cabeçalho e a barra "Falta pagar" mantêm o preto/vermelho da marca.
- O PDF continua sendo gerado pela impressão do navegador ("Salvar como PDF"); o WhatsApp abre a mensagem pronta, sem anexar o arquivo.
