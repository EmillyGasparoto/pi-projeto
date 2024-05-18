# Sistema de gestão universitária

Repositório criado para entrega do Projeto Integrador do Senac. O grupo contém 5 participantes:

- BIANCA LOPES VASCONCELOS 
- ELIENAI TAVARES MATOS DA SILVA 
- ELVIS MATEUS SOUZA DE CARVALHO 
- EMILLY BEATRIZ GASPAROTO 
- KAIO VINICIUS FAGUNDES SANTOS 
- KARILENE DO CARMO FERREIRA 
- NATAN MATEUS BEZERRA DE LIMA 
- WILLIAN RODRIGO DA CRUZ REBOUCAS

## Descrição 

Este projeto propõe um sistema de gestão escolar para cadastro de alunos, professores e fornecedores de
uma universidade.

## Telas

- Cadastro - Permitirá o cadastro de integrantes/forncedores da instituição (professores, alunos e forncedores);
- Login - Permitirá o login dos integrantes da instituição;
- Matrícula em disciplina - Permitirá que o aluno se matricule em disciplinas;
- Consultar Notas - Permitirá que o aluno consulte suas notas do semestre;
- Pagar mensalidade - Permitirá que o aluno pague a mensalidade;
- Atribuir Notas - Permitirá que o professor dê notas aos alunos;
- Planos de Aula - Permitirá que o professor coloque seu plano de aula;
- Registro de Frequência - Permitirá que o professor registre a frequência dos alunos;
- Produtos Fornecidos - Permitirá que o reponsável pelo fornecimento de produtos verifique os produtos fornecidos;
- Faturas - Permitirá o envio de faturas dos produtos fornecidos;
- Atualização de informação - Permitirá alterações e atualizações de informações do fornecedor.

##  Diagramas de casos de uso

left to right direction actor Aluno as "Pessoa Física: Aluno" actor Professor as "Pessoa Física: Professor"
actor Fornecedor as "Pessoa Jurídica: Fornecedor" rectangle "Sistema de Gestão Universitário" {

Aluno -- (Matricular-se em Disciplina)
Aluno -- (Consultar Notas)
Aluno -- (Pagar Mensalidade)
Professor -- (Atribuir Notas)
Professor -- (Criar Plano de Aula)
Professor -- (Registrar Frequência)
Fornecedor -- (Fornecer Produtos)
Fornecedor -- (Enviar Fatura)
Fornecedor -- (Atualizar Informações)

} 

### Descrição do diagrama de casos de uso

- Classe Pessoa: Esta é uma classe abstrata que define atributos comuns a todas as pessoas, como Nome, Endereço e Telefone;
- Pessoa Jurídica (PJ): Subclasse de Pessoa, representa uma pessoa jurídica e possui o atributo CNPJ;
- Aluno (Pessoa Física): Pode se matricular em disciplinas, consultar notas e pagar mensalidades;
- Professor (Pessoa Física): Pode atribuir notas, criar planos de aula e registrar a frequência dos alunos;
- Fornecedor (Pessoa Jurídica): Pode fornecer produtos, enviar faturas e atualizar suas informações;

## Driagrama de Classes










