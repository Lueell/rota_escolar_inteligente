# Rota Escolar Inteligente

### Sistema de Gestão do Transporte Escolar por NFC

**Integrantes**

* Lucas Emanuel da Silva Costa
* Keyte Bel de Souza Nascimento
* João Bosco de Oliveira Neto
* Ysabell Vaneires Ferreira Souza

Instituição: IFRN – Campus Pau dos Ferros

**Trilha escolhida: Eletricidade Instrumental e Programação para Internet.**

## Sobre o Projeto

O Rota Escolar Inteligente é uma proposta de sistema digital desenvolvido para melhorar a organização, o acompanhamento e o controle do transporte escolar utilizado pelos estudantes.

Atualmente, grande parte da comunicação relacionada ao transporte acontece por meio de grupos de WhatsApp, o que pode gerar dificuldades na confirmação dos passageiros, desorganização das informações e problemas no controle de quem realmente utilizará o transporte.

Diante disso, o projeto busca centralizar essas informações em uma única plataforma, oferecendo mais organização e praticidade para estudantes e responsáveis pelo transporte.

**Problema que o Sistema Resolve**

A falta de um sistema centralizado dificulta a organização dos passageiros e o acompanhamento das viagens. A confirmação manual por mensagens pode ocasionar informações desencontradas, atrasos e dificuldades para identificar os alunos que realmente embarcaram.

O sistema busca solucionar esses problemas por meio da confirmação antecipada de viagens, identificação dos estudantes por NFC e acompanhamento da localização dos ônibus por GPS.

**Principais Funcionalidades**

* Cadastro e identificação dos estudantes.
* Confirmação de utilização do transporte para ida e volta.
* Seleção dos pontos de embarque e desembarque.
* Identificação dos alunos por meio de tags NFC.
* Registro automático dos horários de embarque.
* Notificações sobre situações relacionadas à ausência de passageiros.
* Acompanhamento da localização dos ônibus por GPS.

## Protótipo com Inteligência Artificial

O protótipo inicial do sistema foi desenvolvido com auxílio da ferramenta Lovable, utilizando inteligência artificial para auxiliar na criação das interfaces e na estrutura visual da plataforma.

### Telas do Sistema

1. Login <img width="739" height="1600" alt="3f725d5b-7dbc-47d3-9cb9-fac891d17350" src="https://github.com/user-attachments/assets/a1904f63-0619-450f-841f-c848216e8d7b" />


2. Listagem <img width="739" height="1600" alt="7a1ec7c8-bcec-41a4-955b-1e6e76c3ddfe" src="https://github.com/user-attachments/assets/685b26cc-ca76-44ca-86ab-0e9ef6ff76d2" />


3. Detalhes <img width="739" height="1600" alt="7fa5191a-f394-452b-9009-983986471716" src="https://github.com/user-attachments/assets/1506dd12-5245-4efd-9604-26112251bd08" />


4. Cadastro <img width="739" height="1600" alt="da1f5d97-861e-4313-85e3-100bf1ddf5dc" src="https://github.com/user-attachments/assets/bc0a6afd-fbb1-48ff-953c-59a396700320" />

<img width="739" height="1600" alt="5755e718-60e7-4f6a-913b-3793847440cf" src="https://github.com/user-attachments/assets/808a5502-1694-42db-9fb4-fbd2db88c72a" />


Link do protótipo: https://lovable.dev/projects/c43378fd-b8b1-5c57-a16a-22d29204f10c?magic_link=mc_1cf7774c-0501-4f39-ab8c-8912eb5b1b5d

## Modelagem do Banco de Dados

<img width="1251" height="831" alt="rota-escolar-inteligente drawio" src="https://github.com/user-attachments/assets/22470064-e30c-4696-8bbe-ffbe43dab73c" />


O projeto possui um diagrama Entidade-Relacionamento (DER), desenvolvido para representar as entidades, seus atributos e os relacionamentos necessários ao funcionamento do sistema.



## Como Utilizamos Inteligência Artificial

Durante o desenvolvimento do projeto, utilizamos a ferramenta Lovable como auxílio na criação do protótipo da plataforma.

A inteligência artificial foi utilizada para gerar uma estrutura inicial das telas e auxiliar na organização visual do sistema.

### Prompt Utilizado:
Crie um protótipo web, responsivo e com visual limpo, de um Sistema de Gestão do Transporte Escolar para estudantes do IFRN – Campus Pau dos Ferros.

Problema: hoje os alunos combinam o transporte por grupos de WhatsApp, o que gera falta de confirmação organizada de quem vai usar o ônibus, falta de controle de quem realmente embarcou e dependência de mensagens para saber onde o ônibus está. O sistema centraliza isso: o aluno confirma a viagem do dia, o embarque é registrado por tag NFC e o responsável pelo transporte acompanha a lista de passageiros.

Regras: usar apenas dados fictícios no próprio front-end, sem backend, banco de dados nem autenticação real; não implementar NFC nem GPS de verdade — simular com botão "Simular leitura NFC" e mapa ilustrativo; interface toda em português do Brasil; cards com bordas arredondadas e boa legibilidade no celular.

Perfis: aluno (confirma viagens e acompanha o ônibus) e responsável pelo transporte (vê passageiros e registra embarques), com entrada rápida na tela de login.

Telas (mínimo 4):

Login — título do sistema, e-mail, senha, botão Entrar e entrada rápida por perfil.
Listagem de viagens — cards com data, horário, sentido, ônibus, status e alunos confirmados; filtro por data e sentido; ao aluno mostra se ele confirmou, ao responsável mostra confirmados x embarcados.
Detalhe da viagem — mapa ilustrativo com posição do ônibus e previsão de chegada; lista de passageiros com situação ("Confirmado", "Embarcou" ou "Confirmou e não embarcou"); no responsável, "Simular leitura NFC" e "Registrar embarque manual"; no aluno, "Confirmar presença" / "Cancelar confirmação".
Cadastro / confirmação de viagem — formulário com data, trajeto (ir ao IFRN, voltar para a cidade ou ambos), ponto de embarque e ponto de desembarque, com validação dos campos obrigatórios e mensagem de sucesso.
Tela extra: central de notificações com avisos de divergência (ex.: "João confirmou a viagem das 6h30 mas ainda não embarcou").

Dados fictícios: 8 a 10 alunos com nomes brasileiros e cidades da região (Pau dos Ferros, Alexandria, São Miguel, Encanto), 3 ônibus com placas fictícias, 5 a 6 pontos de parada e 4 a 6 viagens entre ida e volta.

Modelo de dados: Usuario, Aluno, Responsavel, TagNFC, Onibus, PontoParada, Viagem, Confirmacao, Embarque, Localizacao e Notificacao.

## O que foi aproveitado:

Ficou do prompt: as quatro telas exigidas (login, listagem, detalhe e cadastro/confirmação), os dois perfis com entrada rápida, a simulação de NFC e de GPS, a validação do formulário de confirmação, a central de notificações com divergências e os dados fictícios seguindo o modelo de entidades.


## O que foi modificado:

Mudou no decorrer do trabalho: a cor principal, que saiu do verde IFRN para amarelo e azul-escuro; a leitura de NFC real pelo celular (Android) foi adicionada como opção, mantendo a simulação e o embarque manual como alternativa; a tela inicial do aluno foi reorganizada com saudação e data, container de confirmação da viagem do dia, acompanhamento por GPS e "Embarques de hoje"; e a página de agendamento passou a ter as quatro opções (ida e volta, só ida, só volta, não vou hoje) com os campos de ponto aparecendo conforme a escolha.

A inteligência artificial foi utilizada como ferramenta de apoio, enquanto as decisões sobre as funcionalidades e os requisitos do sistema foram definidas pelos integrantes.

⸻

## Tecnologias e Ferramentas

* Lovable – criação do protótipo com auxílio de IA.
* GitHub – armazenamento e documentação do projeto.
* Draw.io – elaboração do diagrama do banco de dados.
