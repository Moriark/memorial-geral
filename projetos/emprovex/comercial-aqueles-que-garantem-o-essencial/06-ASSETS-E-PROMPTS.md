# 06 — Plano de assets, pesquisa e prompts de produção

## 1. Diretriz

A geração com IA é **opcional**, não é prova histórica. Combinar imagens licenciadas, filmagens próprias autorizadas, stills tratados e motion design. Toda cena deve ser verificável quanto a direitos e coerência visual. Usar o vídeo da SIGNAL exclusivamente como referência de **ritmo e estrutura**; não cortar/reciclar frames ou áudio da SIGNAL.

## 2. Pacotes de material

| Pacote | Takes | Materiais exigidos | Preferência |
|---|---|---|---|
| A — Antiguidade | T01–T04 | argila, contagem de grãos, armazenamento, transporte | imagens criadas ou licença adequada |
| B — Escrita contábil | T05–T08 | livro-razão, tinta, mão e papel, match cut | captação macro ou material licenciado |
| C — Computação | T09–T13 | calculadora, cartão, mainframe, teclado, dados abstratos | arquivo licenciado + motion |
| D — Aprovisionamento | T14–T23 | prateleiras, etiquetas, conferência, empenho/NF/cronograma fictícios | captação real autorizada prioritária |
| E — Reveal | T24–T30 | transição abstrata, logo oficial, endereço | motion 2D nativo |

**Obter do EMPROVEX:** logo oficial em vetor (SVG/AI) se disponível, PNG de qualidade, regras de marca, domínio correto, screenshot sanitizado opcional para assets de bastidor (não exibir software antes do reveal), fontes oficiais licenciadas.

## 3. Prompts-base para assets visuais (inglês, adaptáveis)

Os prompts abaixo descrevem **cenas originais**, não reproduzem cenas identificáveis de qualquer outro comercial.

### A1 — Argila e registros

“Cinematic macro documentary shot of anonymous ancient hands making tally marks on a clay accounting tablet beside measured grain portions, warm raking light, realistic archaeological material texture, restrained color palette, shallow depth of field, 35mm filmic look, horizontal composition with safe center, no readable modern text, no logo, no watermark, historically plausible setting.”

### A2 — Armazenamento de provisões

“Wide cinematic documentary view of an ancient supply courtyard with baskets and sacks of grain, workers moving provisions, subtle morning dust, realistic natural light, grounded everyday logistics rather than battles, slow dolly perspective, earth tones, no flags or recognizable insignia, no text, no watermark.”

### B1 — Livro e pena

“Extreme close-up of an old ledger being annotated with an ink quill by anonymous hands, diagonal pen stroke intentionally framed to match a diagonal clay mark from previous shot, authentic paper and ink texture, copper shadows, quiet precision, cinematic realism, no readable specific names or monetary claims, no logo.”

### C1 — Máquina de calcular

“Photoreal cinematic macro footage concept of a mid-20th-century mechanical adding machine in operation, tactile metal keys and lever, single hand entering a figure, crisp mechanical action, dramatic but plausible lighting, center framing, no brand logo, no modern touchscreens, no illegible floating UI.”

### C2 — Computação histórica

“Documentary-style wide shot of historical mainframe computing equipment with magnetic tape units in a mid-20th-century computer room, research-accurate styling, technicians as anonymous background silhouettes, controlled practical light, subtle camera glide, no brand logo, no claims of being archival footage.”

### D1 — Depósito contemporâneo

“High-end cinematic documentary shot of an organized supply warehouse for a generic institutional logistics team in Brazil, orderly shelves, labeled neutral boxes, anonymous gloved hands checking items and inventory, natural contemporary lighting, grounded realism, no military insignia, no official endorsement, no sensitive documents, no legible private data.”

### D2 — Aprovisionador e decisão

“Cinematic medium close-up of an anonymous logistics specialist comparing a fictional stock record on a tablet or clipboard with physical packaged supplies, emphasis on hands, focus pull from record to shelf, responsible everyday work, understated emotion and realism, no identifiable person, no logos, no actual procurement data.”

### E1 — Fundo para reveal

“Minimalist cinematic brand-reveal background, almost black with very subtle deep emerald luminous particles converging into a single soft halo, refined premium graphic design, generous central negative space reserved for a genuine logo added later in compositing, no invented wordmark, no fake logo, no text.”

## 4. Requisitos negativos comuns

Sem marcas inventadas, sem braçadeiras/uniformes nacionais reconhecíveis, sem texto pseudo-legível em documentos, sem pessoas famosas, sem armas, sem guerra, sem símbolos oficiais, sem logos de softwares, sem marcas d'água, sem movimentos de mãos anatomicamente absurdos. Corrigir por edição/captação em vez de aceitar distorções visíveis.

## 5. Prompt de movimento por take (modelo)

“Animate this approved still as a subtle 2.5–3 second documentary shot. Preserve identities of objects and all visible labels. Slow 5% camera push-in, natural hand movement only where applicable, realistic depth and stable architecture, no scene mutation, no added text, no new objects, no logos, no morphing between unrelated items. Deliver centered action and clean start/end frames for match cut.”

Para cada take, registrar: asset_id, origem, ferramenta, licença, seed/configuração (se houver), prompt, proprietário, data, resolução, duração, trilha de arquivos e validação humana.

## 6. Bibliotecas e critérios de pesquisa

Pesquisar itens históricos verificáveis em museus, arquivos e bibliotecas com política explícita de uso comercial; procurar imagens de patrimônios arqueológicos de registros de grãos, livros contábeis, calculadoras mecânicas e equipamentos computacionais. **Não presumir domínio público** porque o objeto é antigo — a fotografia, digitalização ou vídeo tem regras próprias.

## 7. Organização local recomendada (fora do Git de texto)

- assets/referencia/ (links e notas de licença, sem copiar conteúdo restrito);
- assets/stills/aprovados/;
- assets/video/gerado/ e assets/video/captado/;
- assets/audio/voz/; assets/audio/musica/; assets/audio/sfx/;
- assets/brand/oficial/;
- edit/animatic/; edit/projeto/;
- exports/master/; exports/social/;
- docs/licenses/ (licenças e termos).

**Importante:** esse layout é uma proposta para armazenamento de mídias; o repositório memorial-geral destina-se a **Markdown** e links. Não adicionar arquivos de mídia grandes sem decidir armazenamento separado.

## 8. Validação de asset antes de entrar na timeline

1. A licença permite edição, uso comercial e distribuição/impulsionamento previstos?
2. A cena não simula falsamente um fato ou local específico?
3. A continuidade entre os takes funciona?
4. Mãos, números, inscrições e arquitetura parecem reais?
5. Não revela informações sensíveis?
6. Está adequada a crop vertical e legendas?
7. Existe a prova de origem/licença registrada?
