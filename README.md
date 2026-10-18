
# Análise Crítica: Estudo de Caso Virtual Case File (VCF) / Sentinel (FBI)

---

## 1. Linha do Tempo Cronológica do Caso

* **1994 / 1995:** Pesquisas do *Standish Group (CHAOS Report)* indicavam que apenas 16% dos projetos de desenvolvimento de software eram concluídos dentro do prazo e do orçamento; 31% eram cancelados e 53% estouravam custos e prazos sem atender às especificações originais.
* **Primavera de 2001:** O FBI contratou a empresa SAIC (*Science Applications International Corporation*) para desenvolver o software do sistema *Virtual Case File* (VCF), como parte do projeto de modernização tecnológica denominado *Trilogy*.
* **Setembro de 2001:** Uma semana antes dos ataques terroristas de 11 de setembro, ocorreu a troca de diretor no FBI (Robert Mueller assumiu no lugar de Louis Freeh). As falhas nos sistemas de informação do FBI contribuíram para a incapacidade de prever os ataques, e a orientação dada foi concluir o desenvolvimento do novo sistema "o mais rápido tecnicamente possível".
* **Final de 2001 / Início de 2002:** O projeto mudou de escopo: em vez de construir uma interface web sobre os sistemas legados já existentes, decidiu-se desenvolver uma solução totalmente nova do zero.
* **Janeiro de 2002:** O FBI solicitou um adicional de US$ 70 milhões ao Congresso para acelerar o projeto *Trilogy* e recebeu US$ 78 milhões, definindo a entrega estimada do VCF para dezembro de 2003.
* **Meados de 2002 (Verão no Hemisfério Norte):** A contratada SAIC dividiu a equipe de desenvolvimento do VCF em 8 grupos paralelos para trabalhar em componentes distintos. A equipe contava com aproximadamente 200 programadores e buscava contratar mais. Surgiram conflitos internos na liderança técnica do projeto (entre Higgins e Patton).
* **Dezembro de 2002:** Higgins solicitou mais US$ 137,9 milhões ao Congresso, sendo aprovados US$ 123,3 milhões (elevando o orçamento total a US$ 581 milhões).
* **2003:** Mais de 400 solicitações de mudança (*change requests*) foram submetidas ao projeto, com grande impacto no escopo e no cronograma.
* **Dezembro de 2003:**
  * Zalmai Azmi assumiu como CIO interino do FBI.
  * A SAIC entregou a versão inicial do VCF, mas o FBI rejeitou a entrega.
  * O FBI documentou 17 falhas/correções necessárias antes do aceite. Houve falta de diálogo com o cliente final ao longo do processo, concentrando as entregas apenas no fim.
* **2004:** Um árbitro neutro foi convocado para julgar a disputa contratual entre o FBI e a SAIC sobre 59 falhas relatadas. O árbitro apontou culpa de ambas as partes: 17 problemas decorriam de mudanças frequentes de requisitos por parte do FBI, e 40 eram defeitos técnicos da própria SAIC.
* **Abril de 2005:** O FBI cancelou oficialmente o projeto *Virtual Case File* (VCF). Foi anunciada a criação do sistema *Sentinel*, orçado em US$ 170 milhões para englobar gestão de casos, evidências e registros.
* **Março de 2006:** Lançamento oficial do projeto *Sentinel* com meta de atender mais de 30.000 agentes e funcionários do FBI. O prazo inicial estimado era dezembro de 2009 com custo total projetado em US$ 451 milhões, estruturado originalmente em quatro fases.
* **Anos Seguintes de Falhas no Sentinel:** O projeto voltou a sofrer com problemas do modelo tradicional (falta de feedback do usuário, requisitos incompletos e oscilantes, falta de apoio executivo, incompetência tecnológica e prazos irrealistas).
* **Virada para o Ágil (Reformulação):** Dois agilistas oriundos do *Lehman Brothers* foram contratados, e o desenvolvimento voltou para dentro do próprio FBI. Foi estruturado o *Scrum Studio* com uma equipe reduzida de apenas 40 desenvolvedores. O projeto reiniciado do zero com a abordagem Ágil foi entregue e finalizado em **1 ano**, com um orçamento de apenas **US$ 30 milhões**.

---

## 2. Respostas às Perguntas

### Por que a abordagem ágil foi utilizada e não a tradicional para o projeto?
A abordagem tradicional (*Waterfall* / Cascata) fracassou repetidamente nos projetos *Trilogy*, *VCF* e nas fases iniciais do *Sentinel* por exigir planejamento rígido e previsibilidade em um ambiente imprevisível. O modelo tradicional gerava ciclos longos sem entregas funcionais, acúmulo de centenas de solicitações de alteração e falta de alinhamento com os agentes do FBI que usariam o sistema. A abordagem ágil foi escolhida para permitir entregas incrementais, feedback constante dos usuários finais e adaptação rápida a mudanças de requisitos.

### Por que o Scrum foi utilizado?
O Scrum offered a estrutura necessária para simplificar a governança do projeto. Em vez de centenas de programadores isolados em múltiplos subgrupos com comunicação deficiente, o Scrum permitiu criar um *Scrum Studio* centralizado com um time enxuto e multidisciplinar (40 desenvolvedores). Ele possibilitou o desenvolvimento focado em *Sprints*, com *Product Owner* definindo prioridades claras e reduzindo o desperdício de tempo e orçamento.

### O resultado final era inovador? Por quê?
**Sim.** O resultado foi inovador tanto do ponto de vista **tecnológico/operacional** quanto de **gestão pública**:
* **Operacional:** Permitiu que mais de 30.000 agentes e analistas do FBI digitalizassem e cruzassem informações de investigações rapidamente em um sistema integrado (gestão de casos, evidências e registros).
* **Gestão de Projetos:** Provou que é possível aplicar metodologias ágeis em um órgão governamental altamente burocrático de grande porte, reduzindo drasticamente custos (de centenas de milhões para US$ 30 milhões) e prazos (de anos para 1 ano).

### O que eu faria diferente?
* **Envolvimento do Usuário desde a Fase 1:** Teria envolvido os agentes de ponta (*end-users*) nos testes desde o início da especificação do sistema, garantindo facilidade de uso e aderência ao fluxo de trabalho real.
* **Evitar o Desenvolvimento do Zero Desnecessário:** Avaliaria a reutilização de módulos dos sistemas existentes em vez de descartar tudo e tentar reescrever o sistema inteiro de uma vez só.
* **Redução da Terceirização Crítica:** Evitaria depender 100% de fornecedores externos sem acompanhamento técnico contínuo e sem entregas parciais de software funcional.

### Outros tópicos interessantes/relevantes?
* **O Paradoxo do Tamanho da Equipe:** No modelo tradicional, a SAIC alocou mais de 200 programadores e o projeto fracassou; no Scrum, uma equipe de apenas 40 desenvolvedores entregou o sistema completo em tempo recorde (demonstrando a *Lei de Brooks*: adicionar mais pessoas a um projeto atrasado o torna ainda mais lento).
* **Custo da Falta de Agilidade:** As falhas de comunicação e a demora na modernização dos sistemas de informação pré-11 de Setembro geraram impactos diretos na segurança nacional.

---

## 3. Links de Referência

* [CSUSB ScholarWorks - Artigo sobre o Estudo de Caso](https://scholarworks.lib.csusb.edu/)
* [Vídeo de Análise do Caso Sentinel / Scrum - YouTube](https://www.youtube.com/watch?v=kNllBLD8k1A&t=328s)
* [Análise Crítica Scrum - Repositório GitHub (Diolemos)](https://github.com/Diolemos/analise-critica-scrum)
