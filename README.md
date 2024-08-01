# Desafio-Tecnico-QA
#
#
## Users Story do módulo de curso do Beedoo
#
## Requerimento 1
#### *Criar padrão de Header*
-Eu- como usuário <br>
-Gostaria- que tivesse um header no site <br>
-Porque- quero que as principais funcionalidades estejam mais visíveis

| Regras de negócio   |                            |                
| ----------------  |:-------------:               |
| 01       | Ter o nome "Beedoo QA Chalenge" no header do lado esquerdo  | 
| 02       | Ter as opções de "LISTAR CURSOS" e "CADASTRAR CURSO" no header, do lado direito, um do lado do outro, e em letras maiúsculas|                         | 
| 03     | O header deverá ter a cor laranja    |
#



## Requerimento 2
#### *Tela de Cadastrar Curso*
-Eu- como usuário <br>
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


























































