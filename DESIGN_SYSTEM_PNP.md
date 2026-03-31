# PNP — PENSANDO COMO EMPRESÁRIO 2.0
## Sistema de Design
> Documento de referência para futura reconstrução do design com IA.

> **Referência de origem:** prints da página de vendas “Aprobado a la primera” (curso de direção em espanhol) enviados como referência visual/inspiração. Embora o produto seja outro, essas páginas foram usadas como direção estética. Toda a análise visual abaixo foi extraída dessas referências.

---

## 1. Estrutura de Layout

### Arquitetura Geral da Página
- **Layout de coluna única em largura total**, com contêineres centralizados usando largura máxima.
- A página é construída como uma **pilha vertical de seções**, cada uma ocupando 100% da largura da viewport.
- Cada seção possui cor/tratamento de fundo próprio, criando separação visual sem depender de bordas.
- Altura média das seções varia bastante — seções hero tendem a ocupar quase a tela inteira (~100vh), enquanto seções de conteúdo ficam na faixa de 400–800px.

### Sistema de Grid
- **Contêiner principal:** aproximadamente 900–1100px de largura máxima, centralizado.
- **Grid de 2 colunas** em seções de benefícios/argumentos, em divisão próxima de 50/50.
- **Grid de 3 colunas** em comparativos e planos.
- **Grid de 4–5 colunas** em fileiras de ícones e tiras de prova social.
- Espaçamento entre colunas: aproximadamente 24–32px.
- Não há linhas visíveis de grid — a estrutura é percebida por alinhamento e espaçamento.

### Tipos de Seção Observados
1. **Barra de navegação** — fixa/sticky, escura ou transparente, logo à esquerda e CTA à direita.
2. **Hero section** — fundo escuro, headline grande alinhada à esquerda, foto do expert à direita, CTA abaixo.
3. **Barra de prova social** — faixa compacta com contagem de alunos e selo de metodologia.
4. **Vídeo + proposta de valor** — fundo escuro, mockup de notebook/tela centralizado, headline acima.
5. **Seção “isso é para você se...”** — mistura de claro/escuro, grid de cards em 2 colunas.
6. **Faixa de benefícios** — ícone + texto curto em linha horizontal.
7. **Bloco de CTA isolado** — botão centralizado entre seções.
8. **Seção de depoimentos/prova social** — prints reais em cards, 3–4 colunas.
9. **Nova faixa de CTA/urgência**.
10. **Tabela comparativa de planos** — 3 colunas com checks e X.
11. **Cards de preço** — 3 planos lado a lado, com nome, preço e CTA.
12. **Faixa de garantia/confiança** — texto curto de segurança.
13. **Seção detalhada de features/conteúdo** — grid/flex com ícones e descrições.
14. **Linha do tempo/plano de estudos** — visual horizontal com opções por cor.
15. **Grid adicional de benefícios** — cards de tamanhos variados.
16. **Bio do expert** — fundo escuro, foto grande à esquerda e texto à direita.
17. **FAQ em accordion** — largura total.
18. **CTA final** — alto contraste com botão grande.
19. **Rodapé** — simples, escuro, texto legal pequeno.

---

## 2. Sistema de Espaçamento

### Escala Inferida
- **Unidade base:** 8px
- **xs:** 8px — microespaçamentos, como ícone para label
- **sm:** 16px — padding interno leve, espaçamento entre elementos inline
- **md:** 24px — entre blocos de texto
- **lg:** 40–48px — padding vertical interno de seções
- **xl:** 64–80px — ritmo vertical entre blocos maiores
- **2xl:** 100–120px — respiros principais, especialmente no hero

### Padrões de Padding
- Seções: 60–80px no topo/baixo e 20–40px nas laterais, dependendo do breakpoint.
- Cards: 24–32px em todos os lados.
- Botões: 14–18px vertical e 28–40px horizontal.
- Navegação: 16px vertical e 24px horizontal.

### Padrões de Margem
- Headline para subheadline: 12–16px
- Subheadline para body copy: 16–20px
- Body copy para CTA: 32–40px
- Entre linhas de features: 16–24px
- Entre seções: **sem margem**; a separação vem da troca de fundo.

---

## 3. Sistema de Cores

### Cores Primárias
| Função | Cor | Hex aproximado |
|---|---|---|
| Vermelho principal da marca | Cor dominante de destaque | `#CC0000` / `#D10000` |
| Vermelho escuro / profundo | Botões e estado ativo | `#990000` / `#A00000` |
| Fundo quase preto | Hero e seções escuras | `#0A0A0A` / `#111111` |
| Cinza carvão escuro | Seções alternadas | `#1A1A1A` / `#1C1C1C` |
| Branco puro | Texto sobre fundo escuro | `#FFFFFF` |
| Branco sujo / cinza claro | Texto secundário e alguns fundos claros | `#F5F5F5` / `#E8E8E8` |

### Cores Secundárias / de Apoio
| Função | Cor | Hex aproximado |
|---|---|---|
| Dourado/areia (plano VIP) | Destaque premium | `#B8975A` / `#C4A355` |
| Verde (check) | Disponibilidade/benefício | `#22C55E` / `#16A34A` |
| Vermelho/rosa (X) | Indisponibilidade | `#EF4444` |
| Âmbar/amarelo | Selo “mais vendido” | `#F59E0B` |

### Tratamento de Fundo
- **Seções escuras:** preto/cinza muito escuro chapado, sem textura.
- **Seções claras:** branco ou cinza muito claro.
- **Alternância dominante:** escuro → claro → escuro → claro.
- **Gradientes:** leves radiais/lineares atrás do expert no hero, com brilho avermelhado.
- **Overlays:** camada escura semitransparente sobre fotos em alguns blocos.

### Regras de Aplicação de Cor
- O vermelho é usado quase sempre com função de conversão: CTA, destaque, urgência, ênfase.
- Texto branco em fundos escuros e texto escuro em fundos claros.
- O dourado é reservado ao plano premium/VIP.
- Verde e vermelho ficam restritos, principalmente, à tabela comparativa.
- A paleta é escura e agressiva; não há tons pastéis, azuis ou roxos.

---

## 4. Tipografia

### Famílias de Fonte Inferidas
- **Fonte de display/headline:** sans-serif pesada, possivelmente condensada ou semi-condensada, com alta presença visual.
- **Fonte de corpo/UI:** sans-serif moderna e neutra, muito legível em tamanhos menores.
- **Fonte de destaque:** normalmente a mesma família da headline, usada com outra cor ou peso.

### Escala Tipográfica Aproximada
| Elemento | Tamanho | Peso | Uso |
|---|---|---|---|
| H1 do hero | 48–72px | 800–900 | Manchete principal |
| H2 de seção | 32–42px | 700–800 | Títulos de blocos |
| H3/subheadline | 22–28px | 600–700 | Apoio |
| Texto de corpo | 15–17px | 400 | Parágrafos |
| Título de card | 14–16px | 600–700 | Cards e listas |
| Texto de botão | 14–16px | 700 | CTA |
| Número de preço | 36–48px | 800 | Valor |
| Badge/tag | 11–13px | 700 | Selos |
| Rodapé/legal | 11–12px | 400 | Informação secundária |

### Regras de Hierarquia Tipográfica
- No máximo 3 escalas tipográficas visíveis por seção.
- A headline sempre domina visualmente.
- Existe técnica de **ênfase parcial** dentro da headline, com 1–2 palavras em vermelho.
- Entrelinhas: ~1.2–1.3 em títulos; ~1.5–1.6 em textos corridos.
- Tracking levemente apertado em títulos; normal no corpo.

---

## 5. Componentes de UI

### Botões CTA
- **Formato:** pílula totalmente arredondada.
- **Variação principal:** fundo vermelho sólido, texto branco, sem borda.
- **Variação secundária:** fundo transparente com borda branca.
- **Tamanho grande:** largura cheia ou ~340px, altura entre 52–60px.
- **Tamanho médio:** ~200–280px, altura entre 44–50px.
- **Ícones:** às vezes seta ou emoji.
- **Fonte:** negrito, caixa alta ou title case.
- **Hover:** vermelho mais escuro e possível leve scale.
- **Apoio abaixo do botão:** ícones de pagamento em linha.

### Cards de Benefícios / Features
- Fundo branco em seções claras e cinza escuro em seções escuras.
- Sem borda aparente; separação por fundo e sombra sutil.
- Bordas arredondadas entre 8–12px.
- Padding de 20–28px.
- Estrutura típica: ícone → título curto → descrição curta.

### Cards de Planos
- 3 colunas lado a lado com larguras semelhantes.
- Card central recebe mais destaque visual.
- Plano VIP recebe cor dourada/areia como diferenciação.
- Estrutura interna: nome do plano → preço original → preço final → CTA → meios de pagamento → nota de garantia.
- Bordas arredondadas entre 10–14px.
- Badge flutuante no plano recomendado.

### Tabela Comparativa
- Tabela em largura total dentro do contêiner central.
- Descrição da feature à esquerda e colunas de comparação à direita.
- Zebra striping sutil.
- Cabeçalhos com nome dos planos.
- Ícone de check em verde e X em vermelho.

### Chips / Pílulas de Benefícios
- Ícone pequeno + texto curto.
- Dispostos em grid horizontal.
- Fundo escuro ou transparente em seção escura.

### FAQ Accordion
- Linhas em largura total.
- Pergunta à esquerda e ícone de expandir à direita.
- Linha divisória entre itens.
- Resposta aparece abaixo quando expandido.

### Navegação
- Barra fixa/sticky.
- Logo à esquerda.
- Links ao centro ou à direita.
- Botão CTA ao extremo direito.
- Transparente sobre o hero e sólida após scroll.

### Prova Social em Prints
- Prints reais de WhatsApp/DM.
- Exibidos como cards com sombra.
- Grid de 3–4 colunas ou composição em mosaico.

### Tira de Fotos
- Fotos levemente inclinadas/estilo polaroid.
- Sobreposição suave.
- Uso puramente de credibilidade visual.

### Tratamento da Foto do Expert
- Foto grande, de alta presença.
- Luz dramática, fundo escuro, color grading puxado para preto/vermelho.
- Não é recorte circular; tende a ocupar boa parte da altura da seção.

### Mockup de Vídeo / Notebook
- Vídeo inserido dentro de moldura de notebook.
- Centralizado.
- Fundo escuro.
- Botão de play como elemento de percepção de valor.

---

## 6. Padrões Visuais

### Padrão do Hero
- Fundo preto/escuro com brilho ou gradiente vermelho.
- Foto do expert à direita com energia e imponência.
- Headline à esquerda em 2–3 linhas.
- 1 ou 2 palavras destacadas em vermelho/laranja.
- Prova social perto da headline.
- CTA imediatamente abaixo.

### Alternância de Contraste
- A página alterna rigidamente entre blocos escuros e claros.
- Isso cria ritmo visual e impede monotonia.

### Ênfase Parcial em Texto
- Headlines usam uma ou duas palavras coloridas no meio da frase para criar hierarquia.
- Essa técnica substitui, em parte, a necessidade de subtítulos muito complexos.

### Densidade de Prova Social
- Alta presença de testemunhos em múltiplos formatos: texto, print, fotos, estrelas e números.

### Selos de Autoridade e Urgência
- Selo de “mais vendido”.
- Contagem de alunos.
- Tags de metodologia validada.

### Separação Entre Seções
- As seções encostam diretamente umas nas outras.
- A separação vem quase toda da mudança de fundo.
- Em alguns pontos, pode existir uma linha/vermelha fina como detalhe decorativo.

---

## 7. Princípios de Design

1. **Estética escura dominante:** o design vive no preto/cinza escuro, com vermelho como acento principal.
2. **Vermelho com função, não decoração:** cada uso de vermelho serve para chamar ação, criar urgência ou destacar algo estratégico.
3. **A fotografia carrega a personalidade:** o expert é o centro da identidade visual.
4. **Prova social em camadas:** o design tenta eliminar objeções usando diversos formatos de confiança.
5. **Tipografia faz o trabalho pesado:** os títulos grandes e fortes conduzem a conversão.
6. **CTA consistente:** o mesmo estilo de botão se repete ao longo da página.
7. **Leitura orientada para mobile:** blocos amplos, botões grandes e hierarquia muito clara.
8. **Respiração controlada:** seções escuras são mais limpas; seções claras comportam maior densidade de informação.
