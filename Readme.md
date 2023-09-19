1.	INTRODUÇÃO E OBJETIVO DO PROJETO INTEGRADOR

Introdução

Dado o exposto, desenvolver um projeto utilizando a Linguagem Unificada de Modelagem (UML) 

Objetivo

Desenvolver um projeto voltado a gestão de dados de um centro universitário onde será construído o diagrama de casos de uso para fazer a representação visual do projeto e o diagrama de classe que é a representação da estrutura e relações das classes que servem de modelo para objetos e logo em seguida fazer a prototipação do projeto para facilitar o entendimento dos requisitos da aplicação 
2.	Diagrama de casos de uso.

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

