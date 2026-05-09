---
description: Gera N variacoes do mesmo prompt em paralelo via sub-agents
---

O usuario quer multiplas variacoes de um mesmo conceito em paralelo. Fluxo:

1. **Identifique a skill** apropriada das 15 do plugin.

2. **Gere o prompt-base** seguindo o framework da skill.

3. **Crie N variantes do prompt** (N entre 2 e 4) variando:
   - Hook (primeiros 2s)
   - Camera move
   - Paleta / lighting
   Mantenha o conceito-central identico nas N variacoes.

4. **Mostre as N variantes** numeradas e pergunte:
   - Aspect ratio
   - Duracao
   - Confirmacao para disparar

5. **Dispare em paralelo** chamando Higgsfield:generate_video N vezes
   simultaneamente (use sub-agents). Cada chamada com count: 1.

6. **Apresente os N resultados** via widget Higgsfield e ofereca:
   - Salvar os melhores prompts em prompts-aprovados/
   - Refinar a partir do que mais agradou
   - Gerar mais N variacoes do escolhido

Lembre o usuario que esse comando consome creditos de forma multiplicada
(N x credito por video). Se o usuario nao confirmou N, pergunte.
