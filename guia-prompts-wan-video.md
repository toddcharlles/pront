# Guia de Prompts Otimizados para Wan.video

## Projeto: Raposa Zod — Canal Crypto/Tutorial

---

## 0. CHARACTER BIBLE — Identidade Visual do Zod (OBRIGATORIO)

> **REGRA NUMERO 1:** Cole o bloco abaixo no INICIO de TODO prompt.
> **REGRA NUMERO 2:** SEMPRE envie a imagem de referencia do Zod junto com o prompt.
> **REGRA NUMERO 3:** NUNCA mude o bloco. Se a IA errar um detalhe, reforce APENAS esse detalhe apos o bloco.

### Bloco Completo (use este por padrao):

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, exaggerated lively gestures, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style.
```

### Bloco Curto (quando o prompt estiver muito longo):

```
Funny energetic orange fox with golden horn, black nerd glasses, gold "Z" chain necklace, fluffy tail, excited goofy expression, childlike squeaky voice, chibi 3D cartoon style.
```

### Detalhes Visuais de Referencia:

| Parte | Descricao Exata |
|-------|----------------|
| Pelo/Fur | Laranja vibrante (bright orange), peito e barriga branco (white chest) |
| Cabeca | Proporcao grande (chibi), chifre dourado pequeno tipo unicornio no topo |
| Olhos | Grandes, escuros, atras dos oculos |
| Oculos | Retangulares, pretos, estilo nerd |
| Nariz | Pequeno, preto |
| Acessorio | Corrente de ouro com medalha/pingente "Z" no pescoco |
| Rabo | Grande, felpudo, laranja |
| Corpo | Proporcoes chibi (cabeca grande, corpo pequeno), bipede |
| Personalidade | ENGRACADO e AGITADO — gestos exagerados, energia alta, expressoes comicas |
| Voz | INFANTIL — childlike high-pitched voice, cute squeaky tone |
| Estilo | 3D cartoon render, ultra realistic cartoon |

### Palavras-chave de Personalidade (adicione conforme a cena):

| Tipo de Cena | Palavras para adicionar |
|--------------|------------------------|
| Apresentando/Tutorial | "funny exaggerated presenter pose, goofy excited expression, childlike enthusiastic voice" |
| Reagindo/Surpreso | "animated lively body language, comedic over-the-top reaction, high-pitched surprised squeak" |
| Dancando/Celebrando | "bouncy energetic movement, playful hyperactive celebration, excited childlike cheering" |
| Explicando | "enthusiastic gestures, comically serious expression, cute squeaky explaining voice" |
| Falando/Narracando | "childlike high-pitched voice, cute squeaky energetic tone, fast excited speech" |

---

## 1. Analise do Prompt que Funcionou

### Prompt original:

> Raposa Zod exata da imagem de referencia, em pe, corpo inteiro, olhando para a camera, pose simpatica de tutorial.
> Ao lado dela (esquerda ou direita, com espaco livre): uma tela monitor grande, quadrada, 100% frontal, perfeitamente paralela a camera, centralizada na composicao, sem inclinacao nenhuma, sem virar para esquerda nem direita, sem diagonal, sem perspectiva 3D, sem angulo, vista reta como se fosse uma parede plana olhando direto para o espectador.
> Tela inteira verde chroma key puro bright green #00FF00, uniforme, sem sombras, sem reflexos, sem distorcao.
> Fundo simples futurista crypto com texto "UNION ZOD" em neon verde grande atras da tela e do Zod.
> Formato 16:9, enquadramento medio, iluminacao flat, ultra realista cartoon, alta qualidade.
> --no angled screen --no tilted monitor --no diagonal view --no perspective distortion --no 3/4 angle --no side view screen --no inclination --no turned left --no turned right

### Por que funcionou (fatores de sucesso):

| Fator | Explicacao |
|-------|-----------|
| Sujeito primeiro | A IA prioriza o que aparece no inicio do prompt |
| Pose definida | "em pe, corpo inteiro, olhando para a camera" elimina ambiguidade |
| Layout espacial | "ao lado dela" define composicao clara |
| Cor exata | "#00FF00" da uma referencia tecnica precisa |
| Estilo consistente | "ultra realista cartoon" e um estilo unico e definido |
| Formato explicito | "16:9" e "enquadramento medio" controlam o frame |

### Problemas identificados (por que outros prompts falham):

| Problema | Impacto |
|----------|---------|
| Repeticao excessiva | Dizer "sem inclinacao, sem virar, sem diagonal, sem perspectiva 3D, sem angulo" 8x confunde a IA — ela foca demais nisso e esquece o resto |
| Sintaxe `--no` e do Midjourney | Wan.video pode ignorar completamente esses flags |
| Instrucoes negativas demais | IAs de video entendem melhor O QUE FAZER do que O QUE NAO FAZER |
| Prompt muito longo | Quanto mais longo, mais a IA "esquece" o inicio |
| Mistura de idiomas | "bright green" + "chroma key" + portugues pode confundir o modelo |

---

## 2. Regras de Ouro para Prompts na Wan.video

### Regra 1: Ordem de prioridade (o que vem primeiro importa mais)
```
1. SUJEITO (quem/o que)
2. ACAO/POSE (o que esta fazendo)
3. COMPOSICAO (onde esta, layout)
4. ESTILO VISUAL (como se parece)
5. DETALHES TECNICOS (formato, iluminacao)
```

### Regra 2: Diga O QUE QUER, nao o que nao quer
```
RUIM:  "sem inclinacao, sem diagonal, sem perspectiva, sem angulo"
BOM:   "monitor perfeitamente frontal, paralelo a camera, vista reta"
```

### Regra 3: Uma instrucao clara > 5 instrucoes repetidas
```
RUIM:  "sem virar para esquerda nem direita, sem diagonal, sem perspectiva 3D, sem angulo, vista reta como se fosse uma parede plana"
BOM:   "monitor frontal plano, exatamente paralelo ao plano da camera"
```

### Regra 4: Use ingles para termos tecnicos universais
```
Wan.video entende melhor termos em ingles para:
- Estilos: "cartoon", "3D render", "flat shading"
- Camera: "medium shot", "front view", "flat lighting"
- Cores: "solid green #00FF00", "chroma key green"
```

### Regra 5: Mantenha o prompt entre 60-120 palavras
```
Menos de 60: falta informacao, IA inventa detalhes
Mais de 120: IA comeca a ignorar partes do prompt
Ponto ideal: 80-100 palavras
```

### Regra 6: Separe elementos com virgulas, nao com frases longas
```
RUIM:  "uma tela monitor grande que seja quadrada e esteja 100% frontal e perfeitamente paralela a camera"
BOM:   "large flat monitor, front-facing, parallel to camera, solid green screen"
```

---

## 3. Estrutura de Prompt Otimizada (Template)

### Template Base:
```
[BLOCO DO PERSONAGEM — copie da secao 0], [POSE], [EXPRESSAO DE PERSONALIDADE].
[LAYOUT/COMPOSICAO DOS ELEMENTOS].
[DETALHES DO CENARIO/OBJETOS].
[ESTILO], [FORMATO], [ILUMINACAO], [QUALIDADE].
```

**IMPORTANTE:** Sempre comece com o Bloco Completo ou Bloco Curto da secao 0.

---

## 4. Prompts Otimizados Prontos para Usar

### PROMPT 1 — Zod com Monitor Chroma Key (versao otimizada do original)

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, exaggerated lively gestures, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style. Full body, looking at camera, funny exaggerated presenter pose.
Large monitor beside character, flat front-facing screen parallel to camera, solid green #00FF00 chroma key fill, clean surface.
Dark futuristic background, neon green "UNION ZOD" text.
Medium shot, 16:9, flat lighting, high quality render.
```

---

### PROMPT 2 — Zod Apresentando (sem monitor, so personagem)

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, exaggerated lively gestures, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style. Full body, facing camera, funny exaggerated presenter pose, one hand gesturing wildly.
Dark futuristic crypto background, neon green glow, "UNION ZOD" text.
Medium shot, 16:9, soft flat lighting, high detail render.
```

---

### PROMPT 3 — Zod com Monitor mostrando Grafico

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, exaggerated lively gestures, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style. Standing beside large flat-screen monitor, enthusiastic tutorial pose, looking at camera.
Monitor facing camera directly, flat front view, screen showing green crypto chart on dark background.
Futuristic dark room, neon green accents, "UNION ZOD" neon sign.
Medium shot, 16:9, flat studio lighting, high quality render.
```

---

### PROMPT 4 — Zod Sentado no Setup Gamer/Crypto

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style. Sitting at futuristic desk, facing camera, comically excited expression, animated lively body language.
Large monitor on desk showing solid green #00FF00 chroma key screen, monitor flat and frontal.
Dark futuristic room, neon green ambient light, crypto aesthetic.
Medium shot, 16:9, cinematic flat lighting, high detail render.
```

---

### PROMPT 5 — Intro/Abertura do Canal

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, exaggerated lively gestures, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style. Full body, dynamic confident pose, arms crossed, big goofy grin at camera.
Dark futuristic environment, holographic crypto symbols floating, large neon green "UNION ZOD" text behind character.
Wide shot, 16:9, dramatic neon lighting, cinematic quality, high detail render.
```

---

### PROMPT 6 — Zod Explicando com Quadro/Tela ao Lado

```
Funny energetic anthropomorphic orange fox character, chibi proportions, big head small body, bright orange fur, white chest fur, small golden unicorn horn on top of head, black rectangular nerd glasses, gold chain necklace with "Z" medallion, big fluffy orange tail, big dark eyes, small black nose, excited goofy expression, exaggerated lively gestures, childlike high-pitched squeaky voice, standing upright on two legs, 3D cartoon render style. Standing, pointing enthusiastically at large floating screen beside him, comedic over-the-top presenter pose.
Floating screen rectangular, front-facing flat, solid bright green #00FF00 chroma key fill, clean surface.
Minimalist dark futuristic background, subtle neon green glow.
Medium shot, 16:9, clean flat lighting, sharp high quality render.
```

---

## 5. Checklist Antes de Enviar um Prompt

Use este checklist para validar qualquer prompt antes de enviar para Wan.video:

- [ ] O personagem esta descrito nas primeiras 10 palavras?
- [ ] A pose e expressao estao claras?
- [ ] O layout/composicao esta definido (quem esta onde)?
- [ ] Usei instrucoes POSITIVAS (o que quero) em vez de negativas (o que nao quero)?
- [ ] O prompt tem entre 60-120 palavras?
- [ ] Nao ha repeticoes da mesma instrucao?
- [ ] Termos tecnicos estao em ingles?
- [ ] O estilo visual esta consistente (nao mistura estilos contraditorios)?
- [ ] Formato (16:9) e iluminacao estao especificados?
- [ ] Nao usei sintaxe de outra plataforma (--no, /imagine, etc)?

---

## 6. Tabela de Traducao: O que Dizer vs O que NAO Dizer

| Voce quer... | NAO diga | DIGA |
|--------------|----------|------|
| Monitor reto | "sem inclinacao, sem diagonal, sem perspectiva" | "monitor flat, front-facing, parallel to camera" |
| Tela verde pura | "sem sombras, sem reflexos, sem distorcao" | "solid uniform green #00FF00, clean flat surface" |
| Personagem olhando pra frente | "sem olhar pro lado, sem virar" | "facing camera directly, eye contact" |
| Fundo simples | "sem muitos detalhes, sem bagunca" | "minimalist dark background, clean composition" |
| Boa qualidade | "sem blur, sem baixa resolucao" | "high detail render, sharp, high quality" |
| Iluminacao uniforme | "sem sombras fortes, sem contrastes" | "flat even lighting, soft studio light" |

---

## 7. Como Adaptar para Novos Videos

Quando precisar de um novo cenario, siga este processo:

1. **Copie o Template Base** (secao 3)
2. **Preencha cada campo** na ordem: personagem > pose > layout > cenario > estilo
3. **Passe pelo Checklist** (secao 5)
4. **Compare com a Tabela de Traducao** (secao 6) para trocar negativos por positivos
5. **Conte as palavras** — ajuste para ficar entre 60-120
6. **Envie para Wan.video**

---

## 8. Notas Sobre Wan.video Especificamente

- **Imagem de referencia:** Sempre envie a imagem do Zod junto com o prompt para manter consistencia
- **Consistencia entre videos:** Use o mesmo bloco de estilo no final de todos os prompts ("Ultra realistic cartoon, medium shot, 16:9, flat lighting, high quality render")
- **Se o resultado nao ficar bom:** Mude UMA coisa por vez no prompt e teste de novo. Nao mude tudo de uma vez
- **Seed/Semente:** Se Wan.video tiver opcao de seed, salve o seed dos resultados bons para reproduzir
- **Resolucao:** Sempre selecione a maior resolucao disponivel na interface
