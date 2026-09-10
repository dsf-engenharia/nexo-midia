# nexo-midia

Fila pública de mídias do Instagram @nexo_intelligence (Nexo Intelligence).
As imagens aqui são as que vão para o feed; por isso o repositório é público.

- `fila.json` — agenda: cada post com `status` (pronto | publicado | sem_legenda), `agendar` (data e hora, horário de Brasília), `image_urls` e `legenda`.
- `posts/<slug>/NN.jpg` — slides 1080x1350 (4:5) em JPEG.
- `posts/<slug>/legenda.txt` — legenda final.

Quem publica: rotina agendada do Claude na nuvem, pelo conector Windsor.ai (Instagram Graph API).
Quem gera a fila: `Marketing/Automacao/nexo_fila.py` no PC da DSF.
