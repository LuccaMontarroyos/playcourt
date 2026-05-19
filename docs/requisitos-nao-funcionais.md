Projeto PlayCourt – Requisitos Não Funcionais e Arquitetura
Disciplina: Processos e Requisitos de Software

Integrantes:

Lucca Pereira
Nome do segundo integrante
1. Introdução

O presente documento apresenta os principais Requisitos Não Funcionais (NFR) do sistema PlayCourt, além da análise de seus impactos arquiteturais e estratégias adotadas para garantir seu funcionamento adequado.

O projeto PlayCourt consiste em um sistema de reserva de quadras esportivas, desenvolvido com o objetivo de facilitar o gerenciamento de horários, reservas e controle das quadras esportivas.

Além das funcionalidades principais do sistema, também foram definidos requisitos não funcionais relacionados a desempenho, segurança, disponibilidade, escalabilidade e usabilidade, buscando garantir qualidade e confiabilidade para os usuários.

2. Requisitos Não Funcionais (NFR)
2.1 Desempenho
Requisito

O sistema deve responder às requisições principais em até 2 segundos para até 500 usuários simultâneos.

Justificativa

Usuários precisam visualizar horários e realizar reservas rapidamente, evitando lentidão durante o processo de agendamento.

Impacto Arquitetural

Esse requisito influencia diretamente a arquitetura do sistema, exigindo:

otimização de consultas ao banco de dados
utilização de cache
controle eficiente de requisições
Estratégias de Mitigação
utilização de cache para consultas frequentes
testes de carga
monitoramento de tempo de resposta
2.2 Segurança
Requisito

O sistema deve garantir autenticação segura dos usuários e proteção dos dados pessoais.

Justificativa

O sistema armazenará informações de usuários e reservas, sendo necessário evitar acessos não autorizados.

Impacto Arquitetural

Esse requisito exige:

autenticação por login e senha
criptografia de senhas
controle de permissões
Estratégias de Mitigação
utilização de hash de senha
validação de autenticação
proteção contra acessos indevidos
2.3 Disponibilidade
Requisito

O sistema deve possuir disponibilidade mínima de 95% do tempo.

Justificativa

Usuários precisam acessar o sistema a qualquer momento para realizar reservas.

Impacto Arquitetural

Esse requisito influencia:

hospedagem do sistema
monitoramento de falhas
recuperação de serviços
Estratégias de Mitigação
monitoramento do servidor
backup periódico
tratamento de falhas
2.4 Escalabilidade
Requisito

O sistema deve suportar crescimento gradual do número de usuários sem perda significativa de desempenho.

Justificativa

O número de usuários pode aumentar conforme mais quadras utilizem o sistema.

Impacto Arquitetural

Esse requisito exige:

arquitetura modular
separação entre frontend e backend
possibilidade de expansão do servidor
Estratégias de Mitigação
utilização de APIs REST
separação de responsabilidades
otimização de recursos
2.5 Usabilidade
Requisito

O sistema deve permitir que usuários realizem reservas em no máximo 3 etapas.

Justificativa

O sistema será utilizado por diferentes perfis de usuários, sendo importante garantir facilidade de uso.

Impacto Arquitetural

Esse requisito influencia:

design da interface
fluxo de navegação
organização das funcionalidades
Estratégias de Mitigação
prototipação de telas
testes de usabilidade
simplificação dos fluxos
3. Relação dos NFR com o Projeto

Os requisitos não funcionais definidos possuem relação direta com o problema identificado no contexto do sistema.

Como o PlayCourt busca organizar reservas de quadras esportivas, é necessário garantir rapidez, disponibilidade e segurança para evitar conflitos de horários, perda de reservas e dificuldades de acesso ao sistema.

Além disso, a usabilidade é fundamental para permitir que usuários consigam utilizar o sistema de forma intuitiva.

4. Decisões Arquiteturais

Com base nos requisitos não funcionais levantados, foram definidas algumas decisões arquiteturais para o sistema:

separação entre frontend e backend
utilização de APIs REST
autenticação de usuários
banco de dados relacional
estrutura modular para facilitar manutenção
possibilidade de uso de cache para otimização de desempenho

Essas decisões contribuem para garantir escalabilidade, segurança e facilidade de manutenção do sistema.

5. Estratégias de Garantia de Qualidade

Para garantir que os requisitos não funcionais sejam atendidos, serão utilizadas as seguintes estratégias:

testes de desempenho
testes de autenticação
monitoramento de falhas
validação das funcionalidades
testes de usabilidade
tratamento de erros e exceções

Essas estratégias ajudam a garantir maior estabilidade e confiabilidade do sistema.

6. Conclusão

A definição dos requisitos não funcionais permitiu identificar aspectos importantes relacionados à qualidade do sistema PlayCourt.

Além das funcionalidades principais, foi possível analisar fatores como desempenho, segurança, disponibilidade e usabilidade, compreendendo como esses elementos impactam diretamente a arquitetura do software.

A atividade contribuiu para o entendimento da importância dos requisitos não funcionais no processo de desenvolvimento de sistemas e na tomada de decisões arquiteturais.
