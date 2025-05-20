# Desafio Técnico – Estágio em Inteligência Artificial · Axur

Este repositório contém a solução completa para o desafio técnico proposto pela Axur, focado em tarefas relacionadas a Inteligência Artificial Multimodal. O desafio avalia competências em scraping, consumo de APIs com autenticação, manipulação de imagens e integração com modelos de linguagem.

---

📌 Objetivo

Automatizar um fluxo que realiza scraping de imagem, envia-a para inferência usando um modelo de IA multimodal, e envia a resposta de volta via API, respeitando autenticação e limites de requisição.

---

🚀 Etapas do Desafio

## ✅ Parte 1 — Execução via Script

1. Scrape da Imagem

- Acesse a URL:
  https://intern.aiaxuropenings.com/scrape/c4087b37-e8b7-4717-8424-8efd3513f995
- Realize o scraping e baixe somente a imagem disponível.

2. Envio para Inferência Multimodal

- Endpoint de API: https://intern.aiaxuropenings.com/v1/chat/completions
- Formato de requisição: padrão da OpenAI API.
- Prompt: <DETAILED_CAPTION>
- Modelo: microsoft-florence-2-large
  - Referência do modelo: https://huggingface.co/microsoft/Florence-2-large
- Autenticação: via token (senha enviada por e-mail)

3. Submissão da Resposta

- Enviar o JSON de resposta recebido (sem alterações) para:
  https://intern.aiaxuropenings.com/api/submit-response
- Usar a mesma autenticação usada na chamada ao modelo.

4. Limite de uso da API

- Máximo de 50 requisições
- Exemplo de visualização: “Requisições feitas para API: 2 de 50 disponíveis.”

## 📤 Parte 2 — Envio Manual do Script

1. Após submissão correta da resposta, atualize a página do desafio via F5.

2. Suba o arquivo com o script utilizado (.py ou .ipynb).

---

🧠 Tecnologias Utilizadas

- Python 3.10+
- Requests
- IPython / Jupyter Notebook
- APIs RESTful
- Autenticação com Bearer Token

---

📁 Estrutura do Projeto

.
├── Axur - Desafio Técnico Estágio IA (Multimodal).ipynb  
├── requirements.txt  
└── README.md

---

⚙️ Como Executar Localmente

1. Clone este repositório:

   git clone https://github.com/seu-usuario/ai-axur-estagio-desafio.git  
   cd ai-axur-estagio-desafio

2. (Recomendado) Crie um ambiente virtual:

   python -m venv venv  
   source venv/bin/activate  # Linux/Mac  
   venv\\Scripts\\activate     # Windows

3. Instale as dependências:

   pip install -r requirements.txt

4. Execute o notebook:

   jupyter notebook "Axur - Desafio Técnico Estágio IA (Multimodal).ipynb"

---

📎 Observações Importantes

- Não modifique o JSON de resposta da IA antes da submissão.
- A senha de autenticação deve ser mantida em segurança e jamais publicada.
- Caso deseje testar localmente, adicione um arquivo .env com sua chave (não incluído no repositório).
- Recomenda-se utilizar menos de 50 chamadas à API durante o desenvolvimento.

---

📬 Contato

Este projeto foi desenvolvido como parte do processo seletivo para estágio em Inteligência Artificial na Axur.

Candidato: Andre Rovai Andrade Xavier Junior  
LinkedIn: https://www.linkedin.com/in/andre-rovai-andrade-xavier-junior-938486178/  
Email: andrerovaijr722@gmail.com
