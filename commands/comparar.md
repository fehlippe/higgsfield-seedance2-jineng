---
description: Compara duas skills do Seedance no mesmo conceito para entender qual rende melhor
---

O usuario quer comparar duas skills do plugin no mesmo conceito-base. Fluxo:

1. **Pergunte qual o conceito-base** (1-2 frases descrevendo a cena/ideia).

2. **Pergunte quais duas skills comparar** entre as 15:
   seedance-cinematic, seedance-3d-cgi, seedance-cartoon, seedance-comic-to-video,
   seedance-fight-scenes, seedance-motion-design-ad, seedance-ecommerce-ad,
   seedance-anime, seedance-product-360, seedance-music-video, seedance-social-hook,
   seedance-brand-story, seedance-fashion-lookbook, seedance-food-beverage,
   seedance-real-estate.

3. **Gere os dois prompts em paralelo** (NAO gere os videos ainda):
   - Use o mesmo conceito-base nas duas
   - Aplique fielmente o framework de cada skill
   - Destaque visualmente o que mudou entre os dois (camera, luz, paletas,
     sound design)

4. **Apresente lado a lado** com um diff conceitual em 3-5 linhas explicando
   as diferencas chave.

5. **Pergunte ao usuario** o que fazer:
   - Gerar so o A
   - Gerar so o B
   - Gerar os dois em paralelo (use sub-agents)
   - Refinar antes de gerar
   - Nada, era so estudo

6. **Se gerar ambos**, dispare em paralelo via Higgsfield:generate_video
   com as mesmas configuracoes (aspect ratio, duracao) para que a comparacao
   seja justa.

Defaults para comparacao: aspect_ratio 9:16, duration 5s, count 1 cada.
