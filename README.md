# BatalhaDeDados-J


## Modelagem e Tratamento de Dados

:blue_book: [Caderno Jupyter com o desenvolvimento da modelagem e tratamento dos dados](modelagem_datavis.ipynb)

Todo processamento foi realizado em Python, usando cadernos Jupyter dentro do ambiente Sagemaker na plataforma da Amazon.
Os dados estavam hospedados em um bucket no S3 da AWS.
Portanto não é possível reproduzir o caderno sem criar a mesma configuração ou sem acesso às fontes originais.

Apesar disso, todas as saídas das células estão visíveis no caderno deste repositório.
Para facilitar, as imagens geradas estão na pasta [graficos_pylot](./graficos_pylot/)


## Sistemas concorrentes 
Do ponto de vista de tratamento e análise de dados educacionais, duas soluções existentes inspiraram nossas propostas:
- a plataforma [SISEDU (Sistema Online de Avaliação, Suporte e Acompanhamento Educacional)](https://sisedu.ced.ce.gov.br/), desenvolvida especificamente para o cenário das escolas estaduais do Ceará
- o trabalho acadêmico ["Junhua Liu et al. Self-Evolving Adaptive Learning for Personalized Education. CSCW '20 Companion. Oct 2020"](https://dl.acm.org/doi/pdf/10.1145/3406865.3418326), uma aplicação estrangeira, denominada SEAL, a qual também busca oferece um sistema de personalização das trajetórias de aprendizagem e de monitoramento inteligente de dados de desempenho dos alunos para professores escolas.

A imagem abaixo mostra um resumo dos nossos estudos preliminares das principais características do SISEDU.
Após conversar com professores e profissionais da rede de educação do Ceará, constatamos que os principais problemas do SISEDU são:
- não ter uma filosofia muito colaborativa para o desenvolvimento de bancos de questões
- não entregar diretamente para o professor os microdados e resultados agregados das estatísticas de desempenho das suas turmas, com os principais resultados de saberes que geraram maiores erros ou dificuldades (aparentemente isso só acontece quando alguém da Secretaria compila os dados e leva a informação para as escolas)
- não ofercer claramente para o professor uma ação sugerida sobre qual estratégia pedagótica ele deve adotar imediatamente após o professor aplicar suas aulas/atividades e coletar os dados de avaliação dos alunos da sua turma.

![SISEDU](https://drive.google.com/uc?export=view&id=1NaUMLb6JcFdzYEeuJdjtKzsU7NbHaIzS)

Já na imagem abaixo, mapeamos as principais características descritas no trabalho estrangeiro do sistema SEAL.
Algumas das soluções propostas no SEAL estão bastante alinhadas com a nossa visão das necessidades e potenciais do sistema ANA.
Entretanto, desconhecemos os detalhes de implementação e difusão do sistema mostrado neste trabalho, ressaltando que é uma publicação bastante recente (divulgada já dentro do período de pandemia).

<img src="https://drive.google.com/uc?export=view&id=1o99MgP_JrlpWJgqFoyvrC1FhZvN9kK3M" alt="SISEDU." width="800px"/> 
