# Documento de Visão — RoboArena

**Disciplina:** Projeto Front-end
**Professor:** Thiago Marcondes Santos
**Turma:** terça de tarde · **Data:** 23/08/2026

> **Aviso:** este documento é um exercício acadêmico da disciplina Projeto
> Front-end. O produto aqui descrito é fictício e serve como exemplo para a
> aplicação das técnicas de levantamento de requisitos vistas em aula
> (brainstorm e 5W2H). Não representa um sistema real, uma empresa real ou
> um evento real.

**Opção escolhida:** Opção 1 — página web sobre um evento universitário.

### Integrantes do grupo

| Nome completo | Matrícula | Seção sob responsabilidade |
|---|---|---|
| Leonardo Mautone | 202601001248 | Capa, seções 6 e 7, anexos e montagem final |
| David Madureira | 202601001345 | 1. Introdução |
| Santiago Alejo | 202601001191 | 2. Posicionamento |
| Joao Duarte | 202601016822 | 3. Envolvidos e usuários |
| Pedro Henrique Godoy | 202602353687 | 4. Visão geral do produto |
| Kaue Reis | 202602576996 | 5. Requisitos de alto nível |
## 1. Introdução

### 1.1 Propósito

Este documento descreve a visão do RoboArena, uma aplicação web para
divulgação, inscrição e acompanhamento de uma competição universitária de
robótica. O objetivo é reunir num único endereço tudo o que hoje está
espalhado entre redes sociais, planilhas e grupos de mensagens, permitindo
que equipes se inscrevam, que a organização gerencie a competição e que o
público acompanhe os confrontos em tempo real.

O documento serve como referência comum para a equipe de desenvolvimento e
para a organização do evento ao longo de todo o projeto, alinhando o que
será construído antes do início da implementação.

### 1.2 Escopo

O RoboArena será uma aplicação web responsiva, acessível por navegador em
computadores e dispositivos móveis.

**Está dentro do escopo:**

- Inscrição de equipes e envio da documentação técnica dos robôs
- Publicação da programação e do regulamento da competição
- Exibição do chaveamento e dos resultados das disputas
- Página individual de cada equipe participante
- Área administrativa para a organização cadastrar equipes e lançar resultados

**Está fora do escopo:**

- Aplicativo nativo para Android ou iOS
- Processamento de pagamento de taxas de inscrição
- Transmissão de vídeo ao vivo das disputas
- Emissão automática de certificados de participação
- Controle de acesso físico ao ginásio

### 1.3 Definições, Acrônimos e Abreviações

| Termo | Significado |
|---|---|
| RoboArena | Nome da aplicação descrita neste documento |
| Chaveamento | Estrutura que organiza os confrontos eliminatórios entre as equipes |
| Equipe | Grupo de estudantes inscrito na competição com um robô |
| Organização | Comissão responsável por realizar o evento e operar a área administrativa |
| RF / RNF | Requisito Funcional / Requisito Não Funcional |
| SPA | Single Page Application — aplicação de página única |
## 2. Posicionamento

### 2.1 Oportunidade de Negócio

A divulgação de eventos universitários acontece hoje pelos canais que os
jovens já frequentam: Instagram, TikTok e murais físicos da instituição.
São canais bons para alcançar público, mas ruins para guardar informação —
o conteúdo se perde no fluxo das publicações e não permite consulta
posterior.

Ao mesmo tempo, o acesso a meios de comunicação pela internet cresceu de
forma constante, e a expectativa de encontrar informação organizada e
disponível a qualquer momento se tornou padrão. Uma plataforma dedicada à
competição atende a essa expectativa, reunindo em um endereço permanente
aquilo que hoje está disperso.

### 2.2 Descrição do Problema

| Item | Descrição |
|---|---|
| O problema de | comunicação e organização dispersas entre redes sociais e murais, sem uma fonte oficial única |
| Afeta | principalmente as equipes que competem |
| Cujo impacto é | conflitos de horário e inconsistência nos dados dos participantes |
| Uma boa solução seria | uma plataforma que ofereça clareza organizacional a todos os participantes, com informação oficial, atualizada e acessível a qualquer momento |

### 2.3 Declaração de Posicionamento

> O RoboArena é uma aplicação web para equipes universitárias que participam
> de competições de robótica e precisam de clareza sobre horários, regras e
> dados de inscrição. Diferente de perfis em redes sociais e murais, ele
> reúne em um único endereço a informação oficial da competição, sempre
> disponível para consulta.
## 3. Descrição dos Envolvidos e Usuários

### 3.1 Resumo dos Envolvidos

| Envolvido | Interesse no sistema | O que espera |
|---|---|---|
| Comissão organizadora | Realizar a competição de forma limpa, segura e bem organizada | Uma fonte oficial que reduza dúvidas e centralize o registro das equipes e dos resultados |
| Professores | Ver seus alunos recebendo reconhecimento acadêmico pelo trabalho desenvolvido | Que o site organize a competição e dê visibilidade a quem se destaca |
| Empresas patrocinadoras | Aproveitar o evento para identificar alunos de destaque | Que os resultados e as equipes fiquem visíveis e acessíveis para consulta |

### 3.2 Resumo dos Usuários

| Perfil | Descrição | Principais necessidades |
|---|---|---|
| Equipes participantes | Grupos de estudantes inscritos na competição com seus robôs | Realizar o registro com as informações exigidas, acompanhar o andamento da competição e consultar o pódio ao final |
| Público e torcida | Pessoas que acompanham a competição presencialmente ou à distância | Consultar o ranking atualizado da competição, acompanhar os confrontos e conferir os resultados |
| Organização (administrador) | Membros da comissão responsáveis pela operação do sistema | Registrar equipes, lançar resultados e pontuações e publicar o pódio |

### 3.3 Necessidades e Expectativas

Entre os perfis atendidos, as equipes participantes são as mais críticas para
o sistema: são elas que sustentam a competição, e é sobre elas que recai o
maior prejuízo quando a informação falha.

Ao mesmo tempo, a necessidade mais frequente durante o evento é a consulta ao
ranking atualizado — tanto pela torcida quanto pelas próprias equipes. Por
isso o RoboArena prioriza dois fluxos: o do competidor, que vai do registro ao
pódio, e o da consulta ao andamento da competição, que precisa estar acessível
a qualquer momento e a partir de qualquer dispositivo.
## 4. Visão Geral do Produto

### 4.1 Recursos Principais

- **Inscrição de equipes:** o competidor preenche um formulário com os dados
  necessários para participação — nome, documento e equipe à qual pertence —
  registrando sua inscrição na competição.

- **Programação e regulamento:** reúne a agenda do evento e o regulamento
  oficial a ser seguido pelos participantes, disponíveis para consulta a
  qualquer momento.

- **Ranking e resultados:** apresenta o ranking atualizado da competição, com
  a tabela de pontuação completa das equipes e dos competidores. É o recurso
  mais consultado durante o evento, tanto pelo público quanto pelas próprias
  equipes.

- **Página da equipe:** exibe os integrantes do time, sua pontuação, suas
  conquistas e as ações mais recentes dentro do torneio.

- **Área administrativa:** permite à organização movimentar pontuações,
  ajustar horários, aplicar punições a competidores ou equipes e atualizar o
  regulamento. As punições são registradas apenas para controle interno da
  organização, sem exibição pública. É o único ponto do sistema em que a
  informação oficial pode ser alterada.

### 4.2 Diferenciais em relação a soluções existentes

Hoje a divulgação de competições universitárias acontece pelas redes sociais
populares entre os jovens. São canais de alcance, não de consulta: a
informação aparece uma vez no feed e depois se perde, e quem precisa de um
dado específico depende de rolar publicações antigas ou perguntar a alguém da
organização.

O RoboArena substitui esse fluxo pela consulta direta. O participante encontra
por conta própria o que precisa — regulamento, programação, pontuação da sua
equipe — sem intermediários e sem depender de quem publicou o quê. E o ranking
se mantém atualizado automaticamente, de modo que a informação vista na tela é
sempre a oficial, no momento em que é consultada.

A diferença central, portanto, é de autonomia: em vez de receber informação
quando alguém decide publicá-la, o usuário busca a informação quando precisa
dela.
## 5. Requisitos de Alto Nível

### 5.1 Requisitos Funcionais

| ID | Requisito | Prioridade |
|---|---|---|
| RF01 | O sistema deve permitir que um competidor realize sua inscrição na competição informando nome, documento e equipe | Alta |
| RF02 | O sistema deve permitir que o usuário consulte os horários da programação do evento | Alta |
| RF03 | O sistema deve permitir que a organização aplique punições a competidores ou equipes pela área administrativa | Alta |
| RF04 | O sistema deve permitir que o usuário consulte o ranking atualizado da competição | Alta |
| RF05 | O sistema deve permitir que o usuário consulte a página individual de uma equipe participante | Média |
| RF06 | O sistema deve permitir que um competidor cancele sua inscrição na competição | Baixa |

### 5.2 Requisitos Não Funcionais

| ID | Requisito | Categoria |
|---|---|---|
| RNF01 | As páginas do sistema devem ser carregadas em até 5 segundos | Desempenho |
| RNF02 | O sistema deve funcionar em dispositivos móveis a partir do padrão de tela e desempenho de aparelhos como Samsung Galaxy S8 e iPhone X | Compatibilidade |
| RNF03 | O sistema deve funcionar nos navegadores Google Chrome, Safari e Microsoft Edge | Compatibilidade |
| RNF04 | A interface deve manter contraste mínimo de 4.5:1 entre texto e fundo, conforme o nível AA da WCAG | Acessibilidade |
| RNF05 | O tamanho mínimo de fonte para texto corrido deve ser de 16px, com altura de linha entre 1.4 e 1.6 | Acessibilidade |
| RNF06 | As informações pessoais dos competidores devem ser armazenadas e transmitidas de forma protegida, acessíveis apenas à organização | Segurança |
| RNF07 | O ranking deve ser atualizado sem que o usuário precise recarregar a página | Desempenho |
## 6. Restrições e Premissas

### 6.1 Restrições

- O prazo para a elaboração deste documento é de uma semana, conforme
  definido pelo professor da disciplina
- O escopo desta etapa se limita à elaboração do documento de visão, sem
  previsão de implementação do sistema descrito
- Caso o sistema venha a ser desenvolvido, deverá utilizar as tecnologias
  adotadas na disciplina: HTML, CSS, JavaScript e React
- O projeto não dispõe de orçamento, devendo ser hospedado em plataforma
  gratuita, como a Vercel
- A disponibilidade da equipe é de aproximadamente uma hora diária por
  integrante, conciliada com as demais disciplinas do semestre

### 6.2 Premissas

- Assume-se que os organizadores do evento fornecerão o regulamento e a
  programação em tempo hábil para publicação no sistema
- Assume-se que os usuários dispõem de dispositivos móveis com navegador
  atualizado, compatíveis com os requisitos definidos na seção 5
- Assume-se a existência de conexão de internet estável no local do evento,
  condição necessária para a consulta ao ranking durante as disputas
- Assume-se que a equipe adquirirá proficiência em React ao longo da
  disciplina, uma vez que nenhum integrante domina a tecnologia no início do
  projeto
## 7. Riscos e Dependências

| Risco / Dependência | Probabilidade | Impacto | Plano de ação |
|---|---|---|---|
| Instabilidade na conexão de internet no local do evento comprometer a consulta ao ranking durante as disputas | Média | Alto | Exibir aviso de indisponibilidade temporária e manter a última pontuação registrada visível até o restabelecimento da conexão |
| Atraso na entrega do regulamento e da programação por parte dos organizadores do evento | Baixa | Alto | Publicar aviso de atraso aos usuários e manter as demais áreas do sistema disponíveis enquanto o conteúdo pendente não é liberado |
| Dificuldade da equipe em cumprir o prazo, agravada por eventual falta de sinergia entre os integrantes | Baixa | Alto | Intensificar a comunicação interna e redistribuir demandas conforme a disponibilidade de cada integrante |
| Integrantes ficarem atrasados nas próprias demandas e o código apresentar falhas por inexperiência com a tecnologia | Média | Médio | Priorizar as funcionalidades essenciais, recorrer à documentação oficial e ao apoio do professor, e revisar em dupla os trechos de maior complexidade |
## 8. Anexo — Técnica Aplicada

### 8.1 5W2H

O levantamento das informações deste documento foi estruturado com a
ferramenta 5W2H, apresentada em aula, cujo preenchimento é apresentado a
seguir.

| Pergunta | Resposta |
|---|---|
| **What?** (O quê?) | Desenvolver a visão de uma aplicação web para uma competição universitária de robótica, reunindo inscrição de equipes, programação, regulamento, ranking e área administrativa em um único endereço |
| **Why?** (Por quê?) | Porque a informação desses eventos hoje circula por redes sociais e murais, canais que alcançam público mas não permitem consulta posterior, gerando falhas de comunicação que afetam principalmente as equipes competidoras |
| **Who?** (Quem?) | O documento foi elaborado pelos seis integrantes do grupo, com divisão por seção. O sistema descrito atende competidores, público e organização do evento, tendo ainda professores e empresas patrocinadoras como envolvidos |
| **Where?** (Onde?) | Aplicação web responsiva, acessível por navegador em computadores e dispositivos móveis, com uso previsto principalmente durante o evento presencial |
| **When?** (Quando?) | O documento de visão foi elaborado no prazo de uma semana definido pelo professor. [Se quiser, acrescente aqui a data de entrega] |
| **How?** (Como?) | Por meio de levantamento colaborativo entre os integrantes, com definição de escopo, perfis de usuário e requisitos funcionais e não funcionais. Caso o sistema venha a ser implementado, serão utilizadas as tecnologias da disciplina: HTML, CSS, JavaScript e React |
| **How much?** (Quanto?) | O projeto não dispõe de orçamento financeiro, prevendo hospedagem em plataforma gratuita. O esforço estimado é de aproximadamente uma hora diária por integrante |
