# Relatório de Processo e Documentação de Vibe Coding

**Landing page de portfólio profissional, do briefing ao refinamento em 3D**

**Autor:** Juan Silva Ribeiro · GitHub: [juansilvarb16](https://github.com/juansilvarb16) · Outubro de 2026

**Ferramentas usadas:** Gemini (estruturação do prompt inicial), Lovable (prototipagem e geração do código, no modo Planejar) e pesquisas em vídeos e referências visuais.

**Link da página:** [Juan Ribeiro — Engenharia de Software, Dados & Automação](https://id-preview--200abaa4-92a8-480d-a550-23f949961ec8.lovable.app/#projetos)

---

## 1. Introdução

Esse relatório conta como eu fiz a minha landing page de portfólio usando vibe coding. A atividade pedia uma página de tema livre, mas deixava claro que o foco não era só o resultado final: o professor queria ver **como eu pensei, como conversei com a IA e como corrigi o caminho** quando algo não saiu como eu esperava. Por isso, em vez de só mostrar a página pronta, organizei aqui todo o processo: a ideia, as decisões de design, os prompts, as pesquisas e a minha avaliação do que a IA entregou.

Segui uma regra simples que chamei de **"Eu primeiro, IA depois"**. Antes de abrir qualquer ferramenta, eu precisava saber o que queria construir e por quê. A IA entrou como executora, e eu fiquei como diretor do projeto.

## 2. Ideação e Briefing

### 2.1 Como comecei

Comecei sem pressa, pensando no que ia fazer. Assisti alguns vídeos sobre como a IA se comporta quando recebe instruções boas e ruins, revisei os slides da aula e li os requisitos com calma. Nessa leitura percebi uma coisa que mudou minha abordagem: como a atividade pedia o registro de todo o processo, resolvi tratar essa landing page como um **teste e treino** para a próxima atividade. Assim eu podia errar, comparar e aprender sem a pressão de entregar algo definitivo.

### 2.2 Por que um portfólio pessoal?

Escolhi o tema **portfólio pessoal interativo** por três motivos:

- **Faz sentido pra mim:** eu vou precisar de um portfólio de qualquer forma, então o exercício serve para algo real.
- **Tem muito espaço visual:** hero, cards, grids, animações. Dá para explorar bastante IDV em uma página só.
- **Tem uma ideia técnica interessante:** imaginei um portfólio onde eu só colo o link do projeto e ele puxa o README e transforma em um botão clicável. Nesta atividade eu decidi fazer **apenas a interface gráfica**, deixando a parte de back-end para uma etapa futura.

### 2.3 Alimentando a IA com meu contexto

Antes de pedir qualquer coisa, comecei a juntar meus dados de carreira (perfil do LinkedIn, GitHub e trajetória) para a IA ter material real e não inventar um perfil genérico. Foi uma decisão importante: quanto mais contexto verdadeiro eu entregava, menos eu precisava corrigir depois.

## 3. Identidade Visual (IDV) e Tokens de Design

Defini a identidade visual antes de gerar código, porque percebi que sem isso a IA escolheria tudo por mim e o resultado ficaria com cara de template. A linha que escolhi foi **dark mode minimalista, elegante, com toque tecnológico e uma pegada editorial**, inspirada em um vídeo de referência com seções numeradas e uma seção "no GitHub".

### 3.1 Paleta de cores

| Token | Cor | Uso e justificativa |
|---|---|---|
| Fundo principal | `#0B0F19` | Azul quase preto. Passa sensação tech sem o cansaço do preto puro. |
| Cards | `#161E2E` | Um tom acima do fundo, cria profundidade sem precisar de bordas pesadas. |
| Texto principal | `#F9FAFB` | Branco suave, com bom contraste e sem estourar na tela escura. |
| Texto secundário | `#9CA3AF` | Cinza para subtítulos e descrições, cria hierarquia de leitura. |
| Destaque | `#6366F1` | Azul/violeta (indigo). Usado em botões, links e brilhos, para guiar o olhar. |

### 3.2 Tipografia

- **Space Grotesk** nos títulos: tem personalidade geométrica e passa o lado tecnológico.
- **DM Sans** no corpo do texto: limpa e muito legível em parágrafos.
- **JetBrains Mono** em tags e detalhes: lembra código e reforça que é um portfólio de desenvolvedor.
- **Caveat** (manuscrita) em uma única frase, "construindo minha jornada na tecnologia": um toque humano no meio de uma página bem técnica.

### 3.3 Conceito editorial

Do vídeo de referência trouxe a ideia de **seções numeradas, muito espaço em branco e textos curtos**. Quis que a página parecesse uma revista tecnológica, não um currículo em formato de site. Escolhi o minimalismo de propósito: se eu enchesse a página de efeitos logo de cara, os cards de projetos (o que realmente importa) perderiam o destaque.

## 4. Comunicação com a IA (Prompts)

Aqui está a parte que mais me ensinou. Em vez de pedir "faça um portfólio bonito", construí a comunicação em **três etapas**, cada uma com um papel diferente.

### 4.1 Etapa 1 — Explicar a ideia de forma simples e pedir um prompt

Peguei alguns exemplos de estrutura de prompt e expliquei minha ideia ao **Gemini** de forma bem direta. Não pedi o site, pedi um **prompt inicial para outra IA construir**. A ideia era usar uma IA para me ajudar a me comunicar melhor com outra. O Gemini devolveu um prompt estruturado, que revisei e aprovei. Os pontos principais dele:

- **Papel definido:** "Atue como um desenvolvedor Front-End sênior especialista em UI/UX".
- **Diretrizes de design (IDV)** com estilo, paleta, tipografia e tokens de cor já especificados.
- **Estrutura da página:** navbar, hero com dois botões ("Ver Projetos" e "Baixar Currículo"), grid de projetos em formato de cards clicáveis e footer com redes sociais.

> Atue como um desenvolvedor Front-End sênior especialista em UI/UX. Vamos criar uma landing page para o meu portfólio profissional de desenvolvimento.
> Estilo: dark mode minimalista, elegante, com toque tecnológico.
> Paleta: fundo #0B0F19, cards #161E2E, texto #F9FAFB / #9CA3AF, destaque #6366F1.
> Tipografia: Inter no corpo, monospace nas tags.
> Estrutura: Navbar, Hero, Projetos (grid de cards), Footer.
> *[resumo do prompt aprovado]*

### 4.2 Etapa 2 — Usar o modo Planejar do Lovable para melhorar a ideia

Levei esse prompt ao **Lovable**, mas em vez de mandar gerar direto, usei a opção **Planejar**. Anexei o texto da ideia base, uma imagem de referência do meu perfil e pedi para ele criar um prompt melhorado, com animações, usando meu LinkedIn e meu GitHub (*juansilvarb16*) como base. Eu queria revisar o plano antes de gastar créditos construindo algo errado.

![Figura 1 — Tela do Lovable no modo Planejar, com o texto da ideia base e a imagem de referência anexados.](imagens/01-lovable-planejar.png)

*Figura 1 — Tela do Lovable no modo Planejar, com o texto da ideia base e a imagem de referência anexados.*

O Lovable devolveu um plano bem mais completo, que aprovei. Entre as melhorias, ele sugeriu:

- Seção **"Fluxo de trabalho"** (ideia, design, código, teste, deploy) com uma linha tracejada que se desenha ao rolar a página.
- Seção **"O que eu faço"** com 6 cards: Front-End, UI/UX, Responsivo, Performance, Integração de APIs e Git/versionamento.
- Seção **"No GitHub"**, que carrega meus repositórios ao vivo pela API do GitHub, com fallback caso a API falhe.
- Animações: revelação ao rolar, barra de progresso no topo, cursor com brilho, botões magnéticos e respeito à opção "reduzir movimento" do sistema.
- Detalhe técnico: framer-motion para animações e React Query para buscar os repositórios.

Uma observação que gostei: o próprio Lovable avisou que **não conseguia ler o LinkedIn automaticamente** e que usaria só o link do perfil, além de deixar claro que os textos de "Sobre" e o link do currículo seriam exemplos. Essa transparência me ajudou a saber o que eu mesmo precisava preencher depois.

### 4.3 Etapa 3 — Prompt de refinamento com efeitos 3D

Com a interface base pronta, olhei o resultado e senti que faltava profundidade. Fui pesquisar efeitos visuais modernos e vi que alguns se encaixavam bem no projeto. Esses efeitos eu já conhecia de nome, mas foram sugeridos durante a criação do prompt e confirmei na pesquisa que combinavam com a identidade tech da página. Escrevi então um prompt de alteração com três pedidos bem específicos:

- **Cards com tilt 3D:** nos projetos, inclinação com `perspective`, `rotateX` e `rotateY` acompanhando o mouse, junto de um brilho dinâmico (spotlight) que segue o cursor.
- **Camadas de profundidade na Hero:** parallax com camadas em velocidades diferentes e `translateZ`, para dar sensação tridimensional.
- **Elemento 3D na Hero (opcional):** um container estilizado na coluna direita, com rotação suave em 3D, deixando aberto o suporte a Spline ou Three.js.

> Atualize o código atual para incorporar efeitos visuais em 3D e maior profundidade na interface:
> 1) Cards com efeito 3D (tilt / perspectiva) + spotlight que segue o cursor.
> 2) Camadas de profundidade na Hero (parallax, translateZ).
> 3) Elemento 3D na Hero com rotação suave (ou embed Spline/Three.js).
> *[resumo do prompt de refinamento]*

Repare que nesse prompt eu não disse "deixa mais bonito". Disse **o que mudar, onde e como**. Essa foi a maior lição de comunicação que levei: prompt específico gera resultado específico.

## 5. Resultado Visual da Página

Os prints abaixo mostram a página publicada rodando, na ordem em que aparecem ao rolar. O link no início do documento leva à versão completa.

![Figura 2](imagens/02-hero.png)

*Figura 2 — Navbar e Hero: título de impacto, frase manuscrita, foto com elemento 3D (cubo girando com tags de tecnologia) e card de status.*

![Figura 3](imagens/03-fluxo-sobre.png)

*Figura 3 — Fluxo de trabalho do dado (fonte, ingestão, bronze/silver/gold, qualidade, consumo) e seção "sobre".*

![Figura 4](imagens/04-o-que-eu-faco.png)

*Figura 4 — Seção "o que eu faço", com cards e tags em fonte monoespaçada.*

![Figura 5](imagens/05-projetos.png)

*Figura 5 — Seção de projetos: cards clicáveis com prévia visual estilizada, tags e ícone de link externo, seguida da seção "stack".*

![Figura 6](imagens/06-github.png)

*Figura 6 — Seção "no github", com repositórios carregados direto da API.*

## 6. Pensamento Crítico e Correção de Caminho

Esse foi o ponto em que mais tentei agir como **diretor do projeto**, e não só como alguém que aperta o botão de gerar.

### 6.1 Como avaliei o que a IA entregou

- **Conferi contra o briefing:** as cores, as fontes e as seções estavam como eu pedi? Os tokens de cor foram respeitados em toda a página?
- **Testei como usuário:** naveguei pela página, passei o mouse nos cards, rolei até o fim e redimensionei a janela para ver o responsivo.
- **Olhei o que era meu e o que era da IA:** textos de "Sobre", projetos em destaque e link do currículo eram de exemplo, então eu sabia que precisava substituir pelos meus dados reais.

### 6.2 Onde corrigi o caminho

A primeira versão estava boa, intuitiva e organizada, mas ainda parecia **plana** para uma página que queria passar a imagem de tecnologia. Em vez de recomeçar do zero, mantive tudo que funcionava e fiz um segundo prompt cirúrgico só com os efeitos em 3D. Também decidi que o elemento 3D da Hero seria opcional: se pesasse ou ficasse exagerado, eu tiraria sem prejudicar o resto.

Outra decisão consciente foi manter o escopo pequeno. A ideia original do portfólio puxar o README automaticamente pelo link do projeto é legal, mas exigiria back-end. Para esta atividade, o objetivo era treinar IDV e comunicação com a IA, então fiquei só na interface e deixei a funcionalidade como evolução futura.

Na versão final também adaptei o conteúdo ao meu perfil real: em vez de focar só em front-end, a página destaca meu caminho em **dados, automação e back-end** (fluxo bronze/silver/gold, projetos como Ocean Sentinel e conciliação automática). Algumas seções ficaram em fundo claro, alternando com o fundo escuro, o que deu ritmo à leitura. Essas mudanças foram decisões minhas durante a revisão.

### 6.3 Humano no comando, IA executando

Resumindo a divisão de papéis: **eu** defini o tema, o escopo, a paleta, as fontes, a referência visual, a estrutura do prompt e decidi o que aprovar. A **IA** escreveu o código, montou os componentes e implementou as animações. Em nenhum momento aceitei o primeiro resultado sem revisar.

## 7. Registro dos Materiais do Processo

- Prompt inicial estruturado (etapa 1)
- Prompt melhorado gerado pelo Lovable no modo Planejar (etapa 2)
- Prompt de refinamento com efeitos 3D (etapa 3)
- Imagem de referência e vídeo de inspiração (perfil e estética editorial)
- Paleta de cores e tokens de tipografia (seção 3)
- Prints da página publicada (seção 5) e link publicado

## 8. Conclusão

Esse projeto era para ser um teste, não a versão final, mas me surpreendeu. Fiquei impressionado com o poder de criação da IA: em pouco tempo saí de uma ideia simples para uma interface com animações, 3D e dados do GitHub ao vivo. Mais importante, entendi que o resultado só ficou bom porque eu sabia o que queria pedir. Quem sabe o que está fazendo enxerga horizontes muito maiores com essas ferramentas, porque a IA amplifica a direção que a gente dá, e quando a direção é fraca ela amplifica isso também.

**O que aprendi:** pensar antes de gerar; definir IDV e tokens antes do código; escrever prompts específicos; usar o modo Planejar para revisar antes de construir; e olhar o resultado com senso crítico.

**Próximos passos:** trocar os textos de exemplo pelos reais, subir meus projetos de verdade e, numa próxima atividade, implementar a ideia do README virando botão clicável.
