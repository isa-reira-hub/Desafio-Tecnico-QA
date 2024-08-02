# DESAFIO QA BEEDOO
#
#



- [Link PLANO DE TESTES](https://docs.google.com/spreadsheets/d/1Z1wQGqIE2y6u2i8rgJ3gJFas5t9npKxA-Mp8ZeWNcUo/edit?usp=sharing)


#
#

## Users Story do módulo de curso do Beedoo
#
## Requerimento 1
#### *Criar padrão de Header*
-Eu- como usuário do Beedoo <br>
-Gostaria- que tivesse um header no site <br>
-Porque- quero que as principais funcionalidades estejam mais visíveis

| Regras de negócio   |                            |                
| ----------------  |:-------------:               |
| 01       | Ter o nome "Beedoo QA Chalenge" no header do lado esquerdo  | 
| 02       | Ter as opções de "LISTAR CURSOS" e "CADASTRAR CURSO" no header, do lado direito, um do lado do outro, e em letras maiúsculas|                         | 
| 03     | O header deverá ter a cor laranja    |
#
#
#

## Requerimento 2
#### *Tela de Cadastrar Curso*
-Eu- como usuário do Beedoo <br>
-Gostaria- de preencher um formulário de cadastro de curso <br>
-Porque- quero adicionar novos cursos à plataforma
#
| Critérios de aceite    |                
| ----------------       |   
| - Nome do curso | 
| - Descrição do curso      |
|  - Instrutor   | 
| - URL da imagem de capa | 
| - Data de início     |
|  - Data de fim  | 
| - Números de vagas | 
| - Tipo de curso    |

#
| Validação de campos    |                
| ----------------       |   
| - O campo "Nome do curso" deve ser obrigatório e conter no máximo 100 caracteres. | 
| - O campo "Descrição do curso" deve ser obrigatório e conter no máximo 1000 caracteres. |
|  - O campo "Instrutor" deve ser obrigatório e conter no máximo 100 caracteres. | 
| - O campo "URL da imagem de capa" deve validar se é uma URL válida. | 
| - Os campos "Data de início" e "Data de fim" devem validar o formato de data (dd/mm/aaaa) e "Data de fim" deve ser posterior à "Data de início". |
| - O campo "Número de vagas" deve aceitar apenas números inteiros positivos.| 
| - O campo "Tipo de curso" deve ser um dropdown (seleção) com opções pré-definidas. |

#
| Mensagem de erro    |                
| ----------------       |   
| - Exibir uma mensagem de erro clara e específica abaixo de cada campo que não atenda aos critérios de validação. | 

#

| Botão de cadastrar curso   |                
| ----------------       |   
| - O botão "Cadastrar Curso" deve estar desabilitado até que todos os campos obrigatórios estejam preenchidos corretamente. | 
| - Ao clicar no botão "Cadastrar Curso", se todos os campos estiverem válidos, o formulário deve ser enviado e o administrador deve receber uma confirmação de sucesso. |
#
| Confirmação de sucesso   |                
| ----------------       |   
| - Após o envio bem-sucedido do formulário, exibir uma mensagem de confirmação indicando que o curso foi cadastrado com sucesso. | 
#
| Design e Usabilidade   |                
| ----------------       |   
| - O formulário deve ser responsivo e funcionar corretamente em dispositivos móveis e desktop. | 
| - O layout deve ser claro e fácil de entender, com etiquetas (labels) apropriadas para cada campo. |

#

| Regras de negócio   |                            |                
| ----------------  |:-------------:               |
| 1. Nome do curso | - O nome do curso deve ser único na plataforma.<br> - Máximo de 100 caracteres. | 
| 2. Descrição do Curso | - Deve fornecer uma visão geral completa do curso<br> - Máximo de 1000 caracteres | 
| 3. Instrutor| - Deve ser um instrutor cadastrado na plataforma<br>Máximo de 100 caracteres.|
| 4. URL da Imagem de Capa| - Deve ser uma URL válida que aponte para uma imagem<br>A imagem deve ser adequada e representar o curso de maneira apropriada | 
| 5. Datas de Início e Fim | - A data de início não pode ser anterior à data atual<br> - A data de fim deve ser posterior à data de início<br> - Ambas as datas devem seguir o formato dd/mm/aaaa | 
| 6. Número de Vagas| - Deve ser um número inteiro positivo<br> - Deve ser maior que zero.|
| 7. Tipo de Curso| - Deve ser selecionado de uma lista de tipos de curso pré-definidos (ex: Presencial, Online, Híbrido)|






#
#
#





## Requerimento 3
#### *Tela Lista de cursos*
-Eu- como usuário do Beedoo <br>
-Gostaria- de visualizar a lista de cursos que já foram criados <br>
-Porque- quero ter acesso de todos os cursos disponíveis na plataforma



| Critérios de Aceitação   |                            |                
| ----------------  |:-------------:               |
| 1. Listagem de Cursos | - A tela deve exibir uma lista de todos os cursos cadastrados<br> - Cada item na lista deve incluir: nome do curso, descrição breve, instrutor, data de início e fim, número de vagas, tipo de curso, e uma imagem de capa | 
| 2. Paginação | - Se o número de cursos exceder um limite predefinido (ex: 10 cursos por página), a tela deve incluir paginação | 
| 3. Opções de Filtro e Pesquisa| - O administrador deve ser capaz de pesquisar cursos pelo nome<br> - O administrador deve ser capaz de filtrar cursos por data de início, data de fim, tipo de curso e instrutor.|
| 4. Ações Disponíveis| - Cada curso na lista deve ter botões para "Editar" e "Excluir"<br> - O botão "Editar" deve permitir que o administrador edite as informações do curso<br> - O botão "Excluir" deve permitir que o administrador remova o curso da plataforma, após confirmação | 
| 5. Design e Usabilidade | - A interface deve ser responsiva, funcionando corretamente em dispositivos móveis e desktop<br> - O layout deve ser claro e fácil de navegar, com etiquetas (labels) apropriadas e botões intuitivos. | 

#

| Regras de Negócio  |                            |                
| ----------------  |:-------------:               |
| 1. Exibição de Informações | - ATodos os cursos devem ser exibidos com informações completas e corretas<br> - A descrição do curso na lista deve ser uma versão abreviada (ex: primeiros 200 caracteres) com uma opção para "ver mais" | 
| 2. Paginação | - A paginação deve ser implementada para melhorar a usabilidade e performance da página<br> - O número de cursos exibidos por página deve ser configurável (ex: padrão 10 cursos por página) | 
| 3. Filtro e Pesquisa| - A pesquisa deve ser insensível a maiúsculas e minúsculas<br> - Os filtros devem ser combináveis para refinar a busca (ex: buscar por nome e filtrar por data)|
| 4. Edição e Exclusão de Cursos| - A edição deve ser feita na mesma tela ou redirecionar para uma tela de edição específica<br> - A exclusão de um curso deve solicitar confirmação para evitar remoções acidentais<br> - Após a exclusão, a lista de cursos deve ser atualizada automaticamente. | 





#
#
#
#
#


| Registro das Decisões |                            |                
| ----------------  |:-------------:               |
| Histórico de Decisões:| - |
| 1. Identificação da Necessidade | - Decisão tomada em reunião de planejamento com stakeholders. <br> - Análise identificada através de um analista UI/UX para definição de figma | 
| 2. Definição do Objetivo do Usuário | - Baseada em entrevistas com administradores e pesquisa de mercado<br> - Validação feita com protótipos e testes de usabilidade | 
| 3. Critérios de Aceitação| - Definidos com o PO/área de negócio e colaboração da equipe de desenvolvimento e QA<br> - Critérios revisados e aprovados por stakeholders| 
| 4. Mockup e Diagrama de Fluxo| - Criados pelo designer UX<br> - Revisados e aprovados em reunião de revisão de design|


































