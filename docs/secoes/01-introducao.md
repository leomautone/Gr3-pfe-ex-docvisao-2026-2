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
