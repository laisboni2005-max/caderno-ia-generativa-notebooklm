# caderno-ia-generativa-notebooklm
# Miniguia de Estudos: Fundamentos de IA Generativa (com NotebookLM)

Contexto e Objetivos

Escolhi Fundamentos de Inteligência Artificial Generativa como tema do meu caderno. Faz sentido pra mim por dois motivos: é um assunto que já uso na prática (inclusive pra construir este próprio projeto) e é um tema cada vez mais cobrado em processos seletivos de TI, então vale a pena entender de verdade o que está por trás da ferramenta, e não só usar no automático.

Objetivos de estudo:
- Entender o que diferencia a IA generativa da IA "tradicional" (preditiva/classificatória).
- Compreender, em linhas gerais, como um modelo generativo aprende e gera conteúdo (padrões, dados de treinamento, prompt).
- Conhecer os principais tipos de IA generativa (texto, imagem, código, áudio) e exemplos de ferramentas de cada tipo.
- Entender os limites e riscos da tecnologia (viés, alucinação, direitos autorais) pra usar com mais consciência crítica.
- Montar um conjunto de prompts reutilizáveis pra revisar o tema rapidamente antes de entrevistas ou provas.

Curadoria de Fontes

Fontes abertas selecionadas e enviadas ao NotebookLM:

1. "O que é IA generativa e para que serve?" (Claranet) — visão geral clara, com comparação entre IA preditiva e IA generativa.
   `https://www.claranet.com/br/blog/o-que-e-ia-generativa-e-para-que-serve`
2. "O que é IA generativa? Definição e exemplos práticos" (Asimov Academy) — explica o conceito com foco didático e exemplos práticos de ferramentas.
   `https://hub.asimov.academy/blog/o-que-e-ia-generativa/`
3. "IA Generativa: o que é, como funciona e aplicações" (Distrito) — traz o histórico da tecnologia (de cadeias de Markov até os LLMs atuais) e aplicações por setor.
   `https://www.distrito.me/blog/o-que-e-a-inteligencia-artificial-generativa`
4. "O que é IA generativa? Definição, exemplos e como funciona" (SAP) — compara IA generativa com IA conversacional e traz a diferença entre IA generativa e AGI.
   `https://www.sap.com/brazil/resources/what-is-generative-ai`
5. "A Inteligência Artificial Generativa no Ecossistema Acadêmico" (artigo acadêmico, arXiv, PDF) — fundamentação conceitual mais formal sobre IA, Machine Learning e IA generativa.
   `https://arxiv.org/pdf/2507.03106`

Todos os links/PDF acima foram carregados como fontes no meu Caderno do NotebookLM.

Engenharia de Prompts e "Cicatrizes"

> Esta seção documenta o processo real de testagem de prompts no NotebookLM. **Preencha com as suas próprias interações** — deixo abaixo o modelo de como estruturar cada entrada, com um exemplo já resolvido pra te guiar.

Exemplo (guia)
- Pergunta inicial: "O que é IA generativa?"
- Resposta obtida (resumo): o NotebookLM trouxe uma definição correta, mas genérica, misturando trechos de duas fontes diferentes sem deixar claro qual dizia o quê.
- Problema encontrado: resposta ampla demais, difícil saber qual fonte embasava cada parte.
- Prompt ajustado: "Com base apenas na fonte da Claranet, explique em até 3 frases o que é IA generativa e cite a diferença em relação à IA preditiva."
- Resultado final: resposta mais objetiva e fácil de citar, com a fonte específica identificada.

### Prompt 1
- Pergunta inicial: "O que é IA generativa?"
- Resposta obtida (resumo): o NotebookLM trouxe uma definição correta, mas juntou trechos de mais de uma fonte sem deixar claro qual dizia o quê — ficou uma resposta ampla, meio "genérica de internet", difícil de citar depois.
- Problema encontrado: eu não conseguia saber qual fonte embasava cada parte da resposta, o que dificulta citar direito num trabalho.
- Prompt ajustado: "Com base apenas na fonte da Claranet, explique em até 3 frases o que é IA generativa e qual a diferença em relação à IA preditiva."
- Resultado final: resposta mais curta, direta e com a fonte identificada — muito mais fácil de reaproveitar no resumo estruturado.

Prompt 2
- Pergunta inicial: "Como a IA generativa funciona por dentro?"
- Resposta obtida (resumo): a resposta ficou muito técnica de uma vez só, misturando conceitos de rede neural, GPU e treinamento sem uma ordem lógica — difícil de acompanhar sem saber o básico antes.
- Problema encontrado: pedir "como funciona" de forma aberta gera uma resposta densa demais pra quem está começando no assunto.
- Prompt ajustado: "Explique como um modelo de IA generativa aprende a gerar conteúdo, em 3 etapas simples, como se fosse para alguém que nunca estudou o assunto."
- Resultado final: a resposta em etapas ficou muito mais didática e virou a base do tópico "Como surgiu" no meu resumo.

Prompt 3
- Pergunta inicial: "Quais são os riscos da IA generativa?"
- Resposta obtida (resumo): o NotebookLM listou riscos bem genéricos ("pode ser perigosa", "precisa de cuidado"), sem trazer exemplos concretos das próprias fontes.
- Problema encontrado: resposta rasa, parecia uma opinião solta em vez de algo embasado nas fontes que eu tinha carregado.
- Prompt ajustado: "Liste, com base apenas nas fontes carregadas, 3 riscos específicos da IA generativa mencionados nos textos, citando de qual fonte vem cada um."
- Resultado final: consegui riscos concretos (desinformação/fake news, questões de propriedade intelectual, viés dos dados) já rastreados até a fonte de origem — isso virou o tópico "Riscos e desafios" do miniguia.

Aprendizados gerais sobre engenharia de prompts no NotebookLM:
- Perguntas muito abertas ("o que é", "como funciona") trazem respostas genéricas e difíceis de citar — pedir "com base apenas na fonte X" resolve isso.
- Pedir a resposta "em etapas" ou "em poucas frases" evita que a IA misture níveis de complexidade diferentes numa resposta só.
- Pedir pra IA identificar a fonte de cada afirmação foi o que mais ajudou no troubleshooting — sem isso, é fácil a resposta parecer opinião solta em vez de algo rastreável.

Miniguia de Estudo

Resumo estruturado

O que é IA generativa
É o ramo da inteligência artificial voltado para criar conteúdo novo — texto, imagem, áudio, vídeo ou código — a partir de padrões aprendidos em grandes volumes de dados. Cada resposta é gerada na hora, moldada pelo comando (prompt) que a pessoa dá.

IA generativa x IA tradicional (preditiva)
A IA "tradicional" costuma ser usada pra classificar ou prever algo com base em dados históricos (ex: prever se um cliente vai cancelar um serviço). Já a IA generativa vai além: em vez de só analisar, ela cria algo novo a partir do que aprendeu.

Como surgiu
A base teórica vem de décadas de pesquisa em estatística e aprendizado de máquina — inclusive de modelos simples, como os que previam a próxima palavra de uma frase com base em probabilidade. Mas a tecnologia só ganhou escala de verdade na última década, quando cresceu o volume de dados disponíveis e o poder computacional das GPUs, permitindo treinar modelos com bilhões de parâmetros.

Tipos e exemplos de ferramentas
- Texto: modelos de linguagem (LLMs) como ChatGPT, Gemini, Claude.
- Imagem: modelos de difusão (como Stable Diffusion, DALL·E e Midjourney) e Redes Generativas Adversariais (GANs), que transformam descrições em ilustrações ou fotos inéditas.
- Código: ferramentas como GitHub Copilot.
- Áudio/vídeo: ferramentas de geração de voz sintética e vídeo a partir de texto.

IA generativa x IA conversacional
A diferença está no objetivo: a IA conversacional foca em manter um diálogo natural com a pessoa, enquanto a IA generativa é mais ampla e cobre a criação de vários tipos de conteúdo, não só texto de conversa.

Riscos e desafios
- Dificuldade de distinguir conteúdo real de conteúdo gerado por IA (desinformação/fake news).
- Questões de propriedade intelectual sobre o conteúdo criado.
- Viés herdado dos dados de treinamento.
- Uso responsável exige checagem humana, principalmente em contextos sensíveis (saúde, jurídico, notícias).

Glossário

IA generativa (GenAI) | Ramo da IA voltado para criar conteúdo novo (texto, imagem, áudio, vídeo, código) a partir de padrões aprendidos |
IA preditiva/tradicional | IA voltada para classificar ou prever resultados com base em dados históricos, sem criar conteúdo novo |
LLM (Large Language Model) | Modelo de linguagem de grande escala, treinado para prever e gerar texto de forma coerente (ex: GPT, Gemini, Claude) |
Prompt | Comando ou instrução em linguagem natural dado à IA para gerar uma resposta |
Rede Neural | Estrutura de aprendizado de máquina inspirada (de forma simbólica) no funcionamento de neurônios, usada para reconhecer padrões |
GAN (Rede Generativa Adversarial) | Arquitetura de duas redes neurais que competem entre si para gerar conteúdo (geralmente imagens) cada vez mais realista |
Modelo de difusão** | Técnica usada por ferramentas como DALL·E e Stable Diffusion para gerar imagens a partir de texto |
Alucinação* | Quando a IA gera uma informação incorreta ou inventada com aparência de resposta confiável |
AGI (Inteligência Artificial Geral) | Conceito (ainda hipotético) de uma IA capaz de igualar ou superar humanos em qualquer tarefa cognitiva |
Machine Learning | Subcampo da IA em que os sistemas aprendem padrões a partir de dados, em vez de seguir regras programadas manualmente |

Prompts reutilizáveis para revisão

Coleção de prompts pra reaproveitar no NotebookLM (ou em qualquer IA) sempre que eu quiser revisar o tema:

1. "Com base apenas nas fontes enviadas, explique em até 5 frases o que é IA generativa e o que a diferencia da IA tradicional."
2. "Crie uma tabela comparando IA generativa, IA preditiva e IA conversacional."
3. "Liste os principais tipos de IA generativa (texto, imagem, código, áudio) com um exemplo de ferramenta para cada um, baseado nas fontes."
4. "Explique, de forma simples, como um modelo de linguagem (LLM) aprende a gerar texto."
5. "Quais são os principais riscos éticos da IA generativa mencionados nas fontes? Liste em tópicos."
6. "Crie 5 perguntas de múltipla escolha sobre os conceitos básicos de IA generativa, usando apenas o conteúdo das fontes."
7. "Monte um glossário com os 10 termos técnicos mais importantes sobre IA generativa mencionados nas fontes."

Ferramentas utilizadas
- [NotebookLM](https://notebooklm.google.com/) — curadoria de fontes e geração de respostas contextualizadas
- Fontes abertas em blogs técnicos e artigo acadêmico (arXiv)
- GitHub — versionamento e publicação do material
