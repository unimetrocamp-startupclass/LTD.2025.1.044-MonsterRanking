# Monster Ranking - README

## 📄 Dados do Cliente
**Projeto:** MonsterRanking: um sistema de engajamento para alunos de academia  
**Cliente:** Academia Corpo Atlético  
**CNPJ/CPF:** 047174330001/13  
**Contato:** (19) 98878-2878  
**E-mail:** eliane.langone@hotmail.com

---

## 👥 Equipe de Desenvolvimento
| Nome                             | Curso                   | Disciplina                                 |
|----------------------------------|--------------------------|---------------------------------------------|
| Lucas Silva do Carmo             | Sistemas de Informação | Padrões de Projetos de Software com Java    |
| João Henrique Augait do Nascimento | Ciências da Computação | Padrões de Projetos de Software com Java    |
| Matheus Azevedo Rosa            | Sistemas de Informação | Padrões de Projetos de Software com Java    |
| Sabrina Ribeiro Guimarães dos Santos | Sistemas de Informação | Padrões de Projetos de Software com Java    |
| Felipe Orpheu Santoro de Vasconcelos | Sistemas de Informação | Padrões de Projetos de Software com Java    |

**Professor Orientador:** Kesede Julio

---

## 📅 1. Introdução
A Academia Corpo Atlético enfrenta baixo engajamento dos alunos com produtos como copos, camisas e luvas. Para solucionar isso, o app Monster Ranking será desenvolvido com desafios, rankings e sistema de pontos, trocáveis por descontos. O app será feito em Flutter com backend em Firebase.

---

## ✨ 2. Objetivo
Aumentar o engajamento dos alunos com os produtos vendidos pela academia através de um app gamificado. Os alunos acumulam pontos participando de desafios e podem trocá-los por recompensas no futuro.

---

## 🔄 3. Escopo
- App Android com 5 telas principais
- Design moderno e intuitivo
- Sistema de ranking dinâmico com base em participação
- Pontos acumulados (sem resgate na versão inicial)

---

## 📆 4. Backlog do Produto
- **Login com Google**: Integração com Firebase Auth para login fácil
- **Ranking dos 3 melhores**: Componente visual em tempo real
- **Sistema de pontuação**: Pontos fixos ao concluir desafios
- **Desafios semanais/mensais**: Exibição e conclusão com botão
- **Perfil editável**: Nome e foto sincronizados com o banco
- **Protótipos no Figma**: Home, Desafios, Ranking, Perfil e Configurações
- **Regras de acesso no Firebase**: Definição de permissões de leitura/escrita

---

## 📅 5. Cronograma da Sprint 2
| Data    | Atividade                                                                 |
|---------|---------------------------------------------------------------------------|
| 21/03   | Início do Sprint 2 e planejamento                                        |
| 22/03   | Criação do card visual do ranking                                        |
| 25/03   | Definição dos itens de backlog iniciais                                 |
| 04/04   | Adição de tarefas de design e regras de Firebase                        |
| 08/04   | Planejamento das regras de segurança                                     |
| 10/04   | Elaboração da versão expandida do escopo                              |
| 11/04   | Consolidação do cronograma da Sprint                                    |

---

## 📓 6. Materiais e Métodos
Link da Modelagem do Sistema: https://drive.google.com/file/d/114MBagQ84uQAI_lknRCmNJ6z2Jw25D8K/view?usp=sharing

**Tecnologias:**
- Flutter, Dart
- Firebase (Auth, Firestore, Rules)
- Figma, Jira, Lucidchart/Draw.io
- Bibliotecas: `firebase_core`, `firebase_auth`, `cloud_firestore`, `google_sign_in`, `provider`, `flutter_hooks`, `flutter_svg`, `google_fonts`

Link da Arquitetura do Sistema: https://drive.google.com/file/d/1XpfvHybYba74oO2aDqLWRD-ondZy6coN/view?usp=sharing

---

## 🔄 7. Resultados

### Protótipo: 
### 🏠 Tela Home
A tela inicial exibe dois carrosséis de cards:
Cards de Ranking: mostram os três primeiros colocados nas votações e rankings de pontuação, com botão para visualizar a lista completa.


Cards de Desafios: destacam os desafios ativos, divididos em categorias como diário, semanal e mensal.


👉 Ações do usuário: visualizar rankings e desafios, clicar em “Ver mais”.
👉 Reações do sistema: carrega os dados do usuário e dos rankings via Firebase e exibe as informações dinamicamente.
		
### 🏆 Tela de Rankings
Essa tela lista todos os usuários ordenados por pontuação acumulada. Também exibe as votações de engajamento, como:
Top 3 maiores fofoqueiros


👉 Ações do usuário: visualizar ranking completo, votar em usuários.
👉 Reações do sistema: votações são armazenadas no Firestore e os resultados atualizados em tempo real.



### 🎯 Tela de Desafios
Mostra todos os desafios disponíveis, com título, descrição e quantidade de pontos. O usuário pode:
Clicar em “Concluir” e ganhar os pontos


Ver seu progresso


👉 Ações do usuário: marcar desafio como concluído.
👉 Reações do sistema: incrementa a pontuação do usuário e altera o botão para "Concluído ✔".


### 👤 Tela de Perfil
Exibe o nome e foto do usuário, bem como sua pontuação atual e botão para editar o perfil.
👉 Ações do usuário: editar nome e foto.
👉 Reações do sistema: dados atualizados no Firebase e refletidos em todo o app.

### Códigos das principais funcionalidades:
Link do trecho de código: https://drive.google.com/file/d/1B4BMo112Litw1CJBYZ6Mil_wF1abJR8K/view?usp=sharing

### 📝 O que esse código faz:
Utiliza um StatefulWidget para permitir a atualização dinâmica da UI.


Armazena uma variável booleana _isCompleted para verificar se o desafio já foi finalizado.


Quando o botão é clicado, a função _handleComplete() atualiza o estado e muda a interface (por exemplo, muda o botão para "✔ Concluído").


---

## 📄 8. Conclusão
**Impacto do sistema:**
- Aumento na interação de pessoas
- Um pequeno aumento na percepção sobre os produtos da Academia

**Melhorias Futuras:**
- Notificações push
- Rankings por categorias (força, cardio, frequência)
- Resgate de pontos por prêmios reais

---

## 🚀 9. Divulgação
link do artigo: https://www.linkedin.com/pulse/monster-ranking-lucas-silva-bg4ue/?trackingId=cysZQoZFSHOImFKjIAMCBQ%3D%3D

A criação de um perfil no LinkedIn para o projeto está prevista, contendo:
- Logo do projeto
- Resumo
- Nomes dos integrantes e orientador
- Publicação de artefatos a cada sprint (diagramas, códigos, artigos)

---

## 10. Carta de Autoriazção e Apresentação
Link: https://drive.google.com/file/d/1kHv1Q1YcboG1UUSTHnys7Et9JveiixE2/view?usp=sharing

---

## 11. Relato Individual
### João Henrique Augait do Nascimento 
Neste relato compartilho minha experiência durante o desenvolvimento de um aplicativo mobile, no qual fui responsável por uma parte essencial do projeto: a construção das interfaces (telas) e a integração com o Firebase.

Desde o início do projeto, envolvi-me ativamente no planejamento e na estruturação da aplicação, focando principalmente na experiência do usuário (UX) e na arquitetura das telas. Utilizei ferramentas modernas de desenvolvimento mobile (como Flutter ), com atenção especial à responsividade, fluidez da navegação e organização visual dos componentes.

A integração com o Firebase foi uma etapa crucial, que exigiu atenção especial à segurança e à eficiência da comunicação entre o app e o backend. Realizei a configuração dos serviços de autenticação (Firebase Auth), banco de dados em tempo real (ou Firestore, conforme o projeto), e também implementei o armazenamento de dados e arquivos. Trabalhei ainda na lógica de autenticação de usuários, leitura e escrita de dados no banco, e controle de sessões.

### Sabrina Ribeiro Guimarães dos Santos
Durante o desenvolvimento de um aplicativo mobile, tive a oportunidade de atuar em várias frentes, cuidando do design, do desenvolvimento e também da organização das tarefas usando o Trello. Foi uma experiência intensa e cheia de aprendizados, na qual assumi responsabilidades importantes em cada etapa do processo.

No design, trabalhei bastante com o Figma para criar as interfaces do app, sempre pensando em como deixá-las bonitas, fáceis de usar e bem organizadas visualmente. Um dos maiores desafios foi desenvolver a tela de usuário, pois precisava garantir uma navegação intuitiva e distribuir bem as informações, para que qualquer pessoa conseguisse usar o aplicativo sem dificuldades.

No desenvolvimento, usei o Flutter, buscando sempre que as telas fossem responsivas e que a navegação fosse suave. Para o backend, contei com o Firebase, onde implementei desde autenticação de usuários até o banco de dados em tempo real, além do armazenamento de arquivos e dados.

Ao longo do projeto, enfrentei alguns desafios técnicos e também ligados à usabilidade. Mas, com bastante teste, ajustes e troca de ideias com a equipe, consegui superar os obstáculos. No fim, a combinação de um design bem pensado, código funcional e a organização das tarefas pelo Trello foi fundamental para que o projeto evoluísse bem.

### Matheus Azevedo Rosa
Esse é um relato pessoal da minha experiência em um projeto de desenvolvimento de um aplicativo mobile. Fiquei responsável por uma parte bem importante: a autenticação de usuários com Firebase, além de criar as telas de login, cadastro, o menu principal e também o primeiro protótipo da integração com o Firebase.

Desde o início, participei ativamente do planejamento e da estrutura do app. Foquei bastante na experiência do usuário e em deixar a navegação entre as telas o mais fluida e intuitiva possível. Usei Flutter durante todo o desenvolvimento, sempre prestando atenção na responsividade e na organização visual dos elementos.

### Lucas Silva do Carmo
Eu tive mais uma boa experiência ao realizar esse projeto, pois foi o momento de colocar em prática os conhecimentos adquiridos nos outros semestres. Fui um dos integrantes responsáveis por cuidar da concepção e estrutura do projeto e acompanhei todas as etapas e processos de desenvolvimento. Além disso, também fiquei responsável por implementar o sistema de pontuação do aplicativo e por estilizar algumas telas, seguindo o protótipo feito no Figma.

Durante a apresentação, consegui falar tudo o que precisava de forma bem natural, o que mostrou uma grande evolução minha em comparação com outras apresentações que já fiz.

No geral, foi uma experiência muito positiva, e espero que no próximo projeto eu consiga fazer ainda melhor.

A parte da integração com o Firebase foi um dos maiores desafios. Tive que configurar os serviços de autenticação (Firebase Auth), banco de dados (Realtime Database ou Firestore, dependendo do que o projeto pedia) e também o armazenamento de dados e arquivos. Além disso, fui eu quem cuidou de toda a lógica de login, leitura e escrita no banco e também do controle de sessões.

Foi uma experiência muito boa, onde aprendi bastante e tive a chance de colocar em prática vários conceitos de mobile e backend na prática.
