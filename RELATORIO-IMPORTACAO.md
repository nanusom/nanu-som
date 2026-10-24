# Relatório da importação de orçamentos — Nanu Som

Gerado em 21/10/2026 a partir dos 27 arquivos PDF enviados (impressões do próprio sistema em nanusom.github.io/nanu-som).

## Resumo

| | |
|---|---|
| PDFs analisados | **27** (todos) |
| Orçamentos distintos (códigos originais) | **23** (nº 0005 a 0027, sem nenhum número faltando) |
| PDFs que repetem o mesmo orçamento com conteúdo diferente | **6** (Lipeh nº 0007: 4 versões; Moraes nº 0011: 2 versões) |
| Registros preparados para importação | **27** (23 principais + 4 versões alternativas) |
| Clientes criados a partir dos orçamentos | **18** |
| Soma dos totais dos 27 registros | R$ 36.902,40 |
| Conferência aritmética | **27 de 27** fecham: soma dos itens = subtotal; subtotal − desconto = total impresso |

Os números 0001 a 0004 não aparecem em nenhum PDF (provavelmente testes ou orçamentos apagados). Nada foi inventado para eles.

## O que acontece em cada navegador (quantos "já existiam")

A contagem de "importados" e "já existiam" **depende do navegador**, porque cada um tem seus próprios dados. O sistema reconhece o que já existe pelo **código original do orçamento** (o mesmo que aparece no endereço `#/orcamento/…`) e, para as versões alternativas, pelo **conteúdo** (cliente + itens + valores).

- **Navegador novo, sem dados (ex.: celular):** entram os 27 registros; nada "já existia".
- **O notebook onde os orçamentos foram criados:** os 23 códigos já existem lá, então os 21 orçamentos que não têm versões alternativas são reconhecidos como já existentes e **não são tocados** (continuam com o status, as edições e as observações que você fez). Para o Lipeh (nº 0007) e o Moraes (nº 0011), o sistema compara cada versão dos PDFs com o que já está no notebook: as que forem **idênticas** são reconhecidas como já existentes; as **diferentes** são adicionadas como orçamentos novos, com número novo acima do maior usado. Nenhum número é repetido.
- O relatório exato de cada navegador aparece em **Configurações → Orçamentos importados** depois da primeira abertura.

Não tenho acesso aos dados que estão hoje no seu navegador, por isso não consigo dizer de antemão quantos serão reconhecidos como duplicados no notebook; o teste que fiz simulou esse caso (um navegador com dados antigos editados e com orçamentos novos): nada foi sobrescrito e nenhum número ficou repetido.

## Casos de duplicidade e como foram tratados

Seis PDFs têm o **mesmo código e o mesmo número**, mas conteúdos (e valores) diferentes. São o mesmo orçamento impresso em momentos diferentes, com opções diferentes. **Como não dá para saber com segurança qual deles é o "oficial", nenhum foi descartado.**

| Orçamento | PDF | Impresso às | Total | Tratamento |
|---|---|---|---|---|
| Lipeh nº 0007 | caixa crua | 08/10 12:23 | R$ 600,00 | versão alternativa (recebe número novo) |
| Lipeh nº 0007 | pintura lisa | 08/10 12:25 | R$ 950,00 | versão alternativa (recebe número novo) |
| Lipeh nº 0007 | pintura no bate pedra | 08/10 12:27 | R$ 700,00 | versão alternativa (recebe número novo) |
| Lipeh nº 0007 | courvin+carpete | 08/10 12:28 | R$ 980,00 | **mais recente: mantém nº 0007 e o código original** |
| Moraes nº 0011 | 4 vias | 09/10 14:35 | R$ 2.110,00 | versão alternativa (recebe número novo) |
| Moraes nº 0011 | trio | 09/10 14:52 | R$ 1.550,00 | **mais recente: mantém nº 0011 e o código original** |

Escolhi a impressão mais recente para ficar com o número original apenas por ser a última; se na prática a oficial for outra, basta apagar as demais no sistema. Cada versão alternativa mostra, na tela do orçamento (e **não** na impressão), de qual PDF veio.

## Lista completa

| PDF | Nº no sistema (navegador novo) | Código original | Cliente | Data | Total | Tratamento |
|---|---|---|---|---|---|---|
| Pablo | 0005 | `xzthouq` | Pablo | 07/10/2026 | R$ 882,40 | Importado com o código e o número originais |
| Samuel | 0006 | `s5qf5hr` | Samuel | 07/10/2026 | R$ 2.100,00 | Importado com o código e o número originais |
| lipeh ( caixa crua ) | 0028 | `etkcy63-v1223` | Lipeh | 08/10/2026 | R$ 600,00 | Versão alternativa do nº 0007 → recebeu o nº 0028 (código etkcy63-v1223) |
| lipeh ( pintura lisa ) | 0029 | `etkcy63-v1225` | Lipeh | 08/10/2026 | R$ 950,00 | Versão alternativa do nº 0007 → recebeu o nº 0029 (código etkcy63-v1225) |
| lipeh ( pintura no bate pedra ) | 0030 | `etkcy63-v1227` | Lipeh | 08/10/2026 | R$ 700,00 | Versão alternativa do nº 0007 → recebeu o nº 0030 (código etkcy63-v1227) |
| lipeh ( courvin+carpete ) | 0007 | `etkcy63` | Lipeh | 08/10/2026 | R$ 980,00 | Versão mais recente do nº 0007 → mantém código e número originais |
| Guilherme | 0008 | `3ibh6la` | Guilherme | 08/10/2026 | R$ 1.675,00 | Importado com o código e o número originais |
| will | 0009 | `vzg6h7c` | will | 09/10/2026 | R$ 660,00 | Importado com o código e o número originais |
| Igor | 0010 | `f8z905o` | Igor | 09/10/2026 | R$ 1.640,00 | Importado com o código e o número originais |
| Moraes 4 vias | 0031 | `bvyibhd-v1435` | Moraes | 09/10/2026 | R$ 2.110,00 | Versão alternativa do nº 0011 → recebeu o nº 0031 (código bvyibhd-v1435) |
| Moraes trio | 0011 | `bvyibhd` | Moraes | 09/10/2026 | R$ 1.550,00 | Versão mais recente do nº 0011 → mantém código e número originais |
| Joo | 0012 | `z14m3c2` | João | 09/10/2026 | R$ 1.560,00 | Importado com o código e o número originais |
| Pedro | 0013 | `e6i53z1` | Pedro | 09/10/2026 | R$ 120,00 | Importado com o código e o número originais |
| Paulinho caixa de grave | 0014 | `r3qcw77` | Paulinho Psound | 13/10/2026 | R$ 1.650,00 | Importado com o código e o número originais |
| Paulinho mdio grave | 0015 | `3rdgnt4` | Paulinho Psound | 13/10/2026 | R$ 600,00 | Importado com o código e o número originais |
| Paulinho corneteira | 0016 | `fgxlmnf` | Paulinho Psound | 13/10/2026 | R$ 375,00 | Importado com o código e o número originais |
| Eduardo Henrique | 0017 | `g3i6p71` | Eduardo Henrique | 13/10/2026 | R$ 1.720,00 | Importado com o código e o número originais |
| Eduardo Felipe | 0018 | `m8c0lqb` | Eduardo Felipe | 13/10/2026 | R$ 1.570,00 | Importado com o código e o número originais |
| Taniel | 0019 | `4w0jie2` | Taniel | 14/10/2026 | R$ 711,00 | Importado com o código e o número originais |
| Taniel 2 | 0020 | `xp0j5gh` | Taniel | 14/10/2026 | R$ 321,00 | Importado com o código e o número originais |
| Andreza | 0021 | `paye5x8` | Andreza | 15/10/2026 | R$ 920,00 | Importado com o código e o número originais |
| Andreza 2 | 0022 | `gm2t3eq` | Andreza | 15/10/2026 | R$ 1.550,00 | Importado com o código e o número originais |
| Moraes 4 vias 2 | 0023 | `m978njp` | Moraes | 17/10/2026 | R$ 2.400,00 | Importado com o código e o número originais |
| Adelson | 0024 | `fheclwh` | Adelson | 17/10/2026 | R$ 3.528,00 | Importado com o código e o número originais |
| Rodrigo | 0025 | `9x6qlkq` | Rodrigo | 17/10/2026 | R$ 1.240,00 | Importado com o código e o número originais |
| Andreza franco | 0026 | `pm7pryq` | Andreza Franco | 17/10/2026 | R$ 1.130,00 | Importado com o código e o número originais |
| Zi | 0027 | `doihhjf` | zi | 17/10/2026 | R$ 3.660,00 | Importado com o código e o número originais |

## Dados preservados e dados que NÃO existem nos PDFs

**Preservados exatamente como estavam nos PDFs:** nome e telefone do cliente (no formato digitado), descrição, quantidade e valor de cada item e de cada caixa, medidas, material, acabamento, observação da caixa, desconto, observações do orçamento e data de emissão.

**Não constam nos PDFs, então não foram preenchidos (nada foi inventado):**
- **Status** do orçamento (Enviado, Aprovado etc.): todos entraram como **Rascunho**, que é o status inicial do sistema. No notebook, que já tem os orçamentos, o status real é mantido.
- **Entrada e saldo restante:** nenhum PDF tem esse valor, exceto uma menção em texto livre no orçamento do Samuel (nº 0006): *"foi dado uma entrada de 100,00"*. O texto das observações foi mantido como está e, **a partir da versão de 22/10**, a entrada de R$ 100,00 também ficou registrada no campo de entrada e marcada como **paga** (valor informado por escrito no próprio orçamento). Nos demais orçamentos não há entrada. Navegadores que já importaram antes dessa versão mantêm o registro antigo do Samuel: abra-o em Editar, informe 100,00 e marque a entrada como paga.
- **Espessura da parede** das caixas (o campo que alimenta a litragem): não aparece nos PDFs. Os campos ficaram vazios; para as caixas com medidas informadas (Samuel, Taniel, Eduardo Henrique e os 3 orçamentos de Paulinho) a litragem calculada internamente só fica correta depois de informar a espessura. A litragem não aparece nos PDFs porque o sistema a oculta do cliente.
- **Caixas sem medidas:** 11 caixas foram impressas como "0 × 0 × 0 cm" (medidas não preenchidas). Entraram sem medidas.
- CPF, e-mail e endereço dos clientes; catálogo de produtos e serviços (os itens dos orçamentos são texto livre; não criei produtos no catálogo).

## Ajustes de leitura dos PDFs (para você conferir)

- Em 9 PDFs apareceu a mensagem "Orçamento salvo" por cima do documento (era o aviso do sistema na hora de imprimir). Removi o aviso.
- **Pablo (nº 0005):** o aviso cobriu o fim de uma frase; reconstruí como *"PREÇO DO FIO PODE TER ALTERAÇAO ATÉ A DATA DE INSTALAÇÃO"*.
- **Igor (nº 0010):** a descrição do primeiro item quebrava em duas linhas no PDF; foi unida em uma só.
- **Observações:** quebras de linha causadas pela largura da página foram unidas; as linhas curtas (listas de equipamentos etc.) foram mantidas separadas.
- O trecho padrão "Orçamento sujeito a alteração de valores…" e o rodapé (telefone e Instagram) vêm das Configurações, então não foram gravados como observação.
- A validade ("Válido por 7 dias") é a mesma em todos e vem das Configurações.

## Onde os dados ficam e como são carregados

1. Os 27 orçamentos e os 18 clientes estão no arquivo **`dados-iniciais.js`** (vai junto no GitHub, ao lado do `index.html`).
2. Na primeira abertura do sistema em cada navegador, o `index.html` lê esse arquivo e **mescla** com os dados que já estão no navegador (`localStorage`, chave `nanusom.v1`). Isso acontece **uma vez por versão do arquivo**; o controle fica na chave `nanusom.v1.dados-iniciais`.
3. Antes de mexer, o sistema guarda uma cópia dos dados que existiam em `nanusom.v1.antes-2026-10-21-1`. Se a gravação falhar, nada é alterado e ele tenta de novo na próxima abertura.
4. Um orçamento importado e depois apagado por você **não volta**.
5. Daí em diante tudo é como antes: os dados ficam só naquele navegador e aparelho; **não são compartilhados** entre notebook e celular. Cada aparelho importa os mesmos 27 registros na sua primeira abertura; o que for criado depois fica só onde foi criado.
