---
description: Gera um video no Seedance 2.0 via Higgsfield usando a skill mais adequada das 15 do plugin
---

Voce vai gerar um video no Seedance 2.0 via Higgsfield. Siga este fluxo:

1. **Identifique a skill correta** entre as 15 disponiveis no plugin:
   seedance-cinematic, seedance-3d-cgi, seedance-cartoon, seedance-comic-to-video,
   seedance-fight-scenes, seedance-motion-design-ad, seedance-ecommerce-ad,
   seedance-anime, seedance-product-360, seedance-music-video, seedance-social-hook,
   seedance-brand-story, seedance-fashion-lookbook, seedance-food-beverage,
   seedance-real-estate.

2. **Anuncie a skill escolhida** e justifique em uma linha. Se houver ambiguidade
   entre 2-3 skills, liste as opcoes e pergunte ao usuario antes de seguir.

3. **Gere o prompt completo** seguindo o framework da skill escolhida (hook de 2s,
   beat-by-beat timeline, camera language, lighting, color grading, audio sync).

4. **Mostre o prompt** ao usuario e pergunte:
   - Aspect ratio (9:16, 16:9, 1:1)
   - Duracao (4 a 15 segundos)
   - Quantidade de variacoes (1 a 4, default 1)

5. **Aguarde confirmacao** antes de disparar.

6. **Dispare a geracao** chamando Higgsfield:generate_video com:
   - model: "seedance_2_0"
   - prompt: prompt completo aprovado
   - aspect_ratio, duration, count conforme escolhido
   - medias: se o usuario subiu imagem/video de referencia, passar com role apropriado

7. **Retorne o resultado** via widget padrao do Higgsfield. Nao resumir o output
   como texto.

Se o pedido do usuario nao se encaixar em nenhuma das 15 skills, diga isso
explicitamente ao inves de improvisar.
