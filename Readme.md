1.	INTRODUÇÃO E OBJETIVO DO PROJETO INTEGRADOR

Introdução

Dado o exposto, desenvolver um projeto utilizando a Linguagem Unificada de Modelagem (UML) 

Objetivo

Desenvolver um projeto voltado a gestão de dados de um centro universitário onde será construído o diagrama de casos de uso para fazer a representação visual do projeto e o diagrama de classe que é a representação da estrutura e relações das classes que servem de modelo para objetos e logo em seguida fazer a prototipação do projeto para facilitar o entendimento dos requisitos da aplicação 
2.	Diagrama de casos de uso.
![Diagrama de casos](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/7ce0df72-4582-48a8-81da-51ec943ffdfa)

3.	Cenários de casos de usos

3.1	Registrar Pessoa Física
Descrição: Este caso de uso permite que o sistema registre uma pessoa física no sistema escolar.
     Pré-condições: O usuário deve ter acesso ao sistema de gestão escolar.
     Fluxo principal:
     O usuário seleciona a opção de registrar pessoa física no sistema.
     O sistema solicita as informações necessárias, como nome e CPF.
     O usuário insere as informações da pessoa física.
     O sistema valida as informações e registra a pessoa física no sistema.
     Pós-condição: A pessoa física é registrada com sucesso no sistema escolar.

Cenário Alternativo 1: Dados inválidos
    No passo O sistema valida as informações e registra a pessoa física no sistema do fluxo principal, o sistema detecta que os dados fornecidos são inválidos.
    O sistema exibe mensagens de erro ao lado dos campos correspondentes.
    O usuário corrige os dados inválidos.
    O usuário clica no botão de enviar novamente.
    O sistema valida as informações corrigidas e registra a pessoa física no sistema.
 Pós-condição: A pessoa física é registrada com sucesso no sistema escolar, após a correção dos dados inválidos.

Cenário Alternativo 2: Cancelar o registro
  Fluxo alternativo:
    No passo O usuário insere as informações da pessoa física, o usuário decide cancelar o registro da pessoa física.
    O usuário clica no botão de cancelar.
    O sistema cancela o registro em andamento e retorna à página anterior.
  Pós-condição: O sistema não registra a pessoa física e retorna à página anterior.


3.2 Registrar Pessoa Jurídica

Este caso de uso permite que o sistema registre uma pessoa jurídica no sistema escolar.
     Pré-condições: O usuário deve ter acesso ao sistema de gestão escolar.
     Fluxo principal:
     O usuário seleciona a opção de registrar pessoa jurídica no sistema.
     O sistema solicita as informações necessárias, como nome fantasia e CNPJ.
     O usuário insere as informações da pessoa jurídica.
     O sistema valida as informações e registra a pessoa jurídica no sistema.
     Pós-condição: A pessoa jurídica é registrada com sucesso no sistema escolar.

Cenário Alternativo 1: Dados inválidos
  Fluxo alternativo:
  No passo O sistema valida as informações e registra a pessoa jurídica no sistema do fluxo principal, o sistema detecta que os dados fornecidos são inválidos.
  O sistema exibe mensagens de erro ao lado dos campos correspondentes.
  O usuário corrige os dados inválidos.
  O usuário clica no botão de enviar novamente.
  O sistema valida as informações corrigidas e registra a pessoa jurídica no sistema.
  Pós-condição: A pessoa jurídica é registrada com sucesso no sistema escolar, após a correção dos dados inválidos.

Cenário Alternativo 2: Cancelar o registro
  Fluxo alternativo:
  No passo O usuário insere as informações da pessoa jurídica do fluxo principal, o usuário decide cancelar o registro da pessoa jurídica.
  O usuário clica no botão de cancelar.
  O sistema cancela o registro em andamento e retorna à página anterior.
  Pós-condição: O sistema não registra a pessoa jurídica e retorna à página anterior.
3.3 Registrar Professor

   	Este caso de uso permite que o sistema registre um professor no sistema escolar.
     Pré-condições: O usuário deve ter acesso ao sistema de gestão escolar e a pessoa física relacionada ao professor deve estar registrada no sistema.
     Fluxo principal:
     O usuário seleciona a opção de registrar professor no sistema.
     O sistema exibe uma lista de pessoas físicas registradas no sistema.
     O usuário seleciona a pessoa física correspondente ao professor.
     O sistema solicita informações adicionais, como matrícula, área e disciplina.
     O usuário insere as informações do professor.
     O sistema valida as informações e registra o professor no sistema.
     Pós-condição: O professor é registrado com sucesso no sistema escolar.

Cenário Alternativo 1: Professor não encontrado na lista

  No passo O usuário seleciona a pessoa física correspondente ao professor do fluxo principal, o usuário não encontra a pessoa física correspondente ao professor na lista exibida pelo sistema.
  O usuário seleciona a opção de cadastrar uma nova pessoa física.
  O sistema direciona o usuário para o caso de uso "Registrar Pessoa Física".
  O usuário cadastra uma nova pessoa física.
  O sistema volta ao fluxo principal no passo 4.
  O usuário insere as informações adicionais do professor.
  O sistema valida as informações e registra o professor no sistema.
  Pós-condição: O professor é registrado com sucesso no sistema escolar, juntamente com a nova pessoa física cadastrada.

Cenário Alternativo 2: Dados adicionais inválidos
  Fluxo alternativo:
  No passo O sistema valida as informações e registra o professor no sistema do fluxo principal, o sistema detecta que os dados adicionais fornecidos são inválidos.
  O sistema exibe mensagens de erro ao lado dos campos correspondentes.
  O usuário corrige os dados inválidos.
  O usuário clica no botão de enviar novamente.
  O sistema valida as informações corrigidas e registra o professor no sistema.
  Pós-condição: O professor é registrado com sucesso no sistema escolar, após a correção dos dados adicionais inválidos.


3.4 Registrar Fornecedor

     Descrição: Este caso de uso permite que o sistema registre um fornecedor no sistema escolar.
     Pré-condições: O usuário deve ter acesso ao sistema de gestão escolar e a pessoa jurídica relacionada ao fornecedor deve estar registrada no sistema.
     Fluxo principal:
     O usuário seleciona a opção de registrar fornecedor no sistema.
     O sistema exibe uma lista de pessoas jurídicas registradas no sistema.
     O usuário seleciona a pessoa jurídica correspondente ao fornecedor.
     O sistema solicita informações adicionais, como código, produto e serviço fornecido.
     O usuário insere as informações do fornecedor.
     O sistema valida as informações e registra o fornecedor no sistema.
     Pós-condição: O fornecedor é registrado no sistema


Cenário Alternativo 1: Fornecedor não encontrado na lista
  Fluxo alternativo:
   No passo O usuário seleciona a pessoa jurídica correspondente ao fornecedor do fluxo principal, o usuário não encontra a pessoa jurídica   correspondente ao fornecedor na lista exibida pelo sistema.
  O usuário seleciona a opção de cadastrar uma nova pessoa jurídica.
  O sistema direciona o usuário para o caso de uso "Registrar Pessoa Jurídica".
  O usuário cadastra uma nova pessoa jurídica.
  O sistema volta ao fluxo principal no passo 4.
  O usuário insere as informações adicionais do fornecedor.
  O sistema valida as informações e registra o fornecedor no sistema.
  Pós-condição: O fornecedor é registrado no sistema escolar, juntamente com a nova pessoa jurídica cadastrada.

Cenário Alternativo 2: Dados adicionais inválidos
  Fluxo alternativo:
  No passo O sistema valida as informações e registra o fornecedor no sistema do fluxo principal, o sistema detecta que os dados adicionais fornecidos são inválidos.
  O sistema exibe mensagens de erro ao lado dos campos correspondentes.
  O usuário corrige os dados inválidos.
  O usuário clica no botão de enviar novamente.
  O sistema valida as informações corrigidas e registra o fornecedor no sistema.
  Pós-condição: O fornecedor é registrado no sistema escolar, após a correção dos dados adicionais inválidos.
  3.5 Registrar Aluno

  	Este caso de uso permite que o sistema registre um aluno no sistema escolar.
  Pré-condições: O usuário deve ter acesso ao sistema de gestão escolar.
 O usuário seleciona a opção de registrar aluno no sistema.
 O sistema solicita as informações necessárias, como nome, CPF e curso.
 O usuário insere as informações do aluno.
 O sistema valida as informações e registra o aluno no sistema.
 Pós-condição: O aluno é registrado com sucesso no sistema escolar.

Cenário Alternativo 1: Dados inválidos
  Fluxo alternativo:
  No passo O usuário insere as informações do aluno do fluxo principal, o sistema detecta que os dados fornecidos são inválidos.
  O sistema exibe mensagens de erro ao lado dos campos correspondentes.
  O usuário corrige os dados inválidos.
  O usuário clica no botão de enviar novamente.
  O sistema valida as informações corrigidas e registra o aluno no sistema.
  Pós-condição: O aluno é registrado com sucesso no sistema escolar, após a correção dos dados inválidos.

Cenário Alternativo 2: Cancelar o registro
  Fluxo alternativo:
  No passo O usuário insere as informações do aluno do fluxo principal, o usuário decide cancelar o registro do aluno.
  O usuário clica no botão de cancelar.
  O sistema cancela o registro em andamento e retorna à página anterior.
  Pós-condição: O sistema não registra o aluno e retorna à página anterior.

![diagrama de classe](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/63d96f3e-383c-4967-99c0-1cdaccead3a4)

![pagina de cadastro](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/8ca90284-1a2d-4d20-bab4-d490cd0934be)

![cadastro de alunos](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/2f57469c-5b64-428b-adb7-6d77e51f7ed9)

![Cadastro de pessoas fisicas](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/6e3a370b-7e1d-46fb-9c99-0f96b533f36e)

![cadastro de pessoas juridicas](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/91d776fe-3347-492c-9384-e534ec9fc25e)

![Cadastro Fornecedor](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/f391e657-bdb8-47e0-8511-8a5d2cb74668)

![Cadastrol de professores](https://github.com/gruposenac33/Projeto-integrador/assets/144973922/a2526f76-950d-4fce-88b7-cb3046095538)
