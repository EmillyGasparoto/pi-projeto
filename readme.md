# Sistema de gestão universitária

Repositório criado para entrega do Projeto Integrador do Senac. O grupo contém 8 participantes:

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

- Login/Cadastro - Permitirá o login e cadastro dos integrantes e fornecedores da instituição;
- Matrícula em disciplina - Permitirá que o aluno se matricule em disciplinas;
- Consultar Notas - Permitirá que o aluno consulte suas notas do semestre;
- Pagar mensalidade - Permitirá que o aluno pague a mensalidade;
- Atribuir Notas - Permitirá que o professor dê notas aos alunos;
- Planos de Aula - Permitirá que o professor coloque seu plano de aula;
- Registro de Frequência - Permitirá que o professor registre a frequência dos alunos;
- Produtos Fornecidos - Permitirá que o reponsável pelo fornecimento de produtos verifique os produtos fornecidos;
- Faturas - Permitirá o envio de faturas dos produtos fornecidos;
- Atualização de informação - Permitirá alterações e atualizações de informações do fornecedor.

### Login/Cadastro

Tela responsável por validar login, senha, e fazer o cadastro de usuários.

![Tela de Login/Cadastro](/prototipo-pi-imagem/1.jpg)

### Página do Aluno

Área exclusiva do aluno para matricular-se em disciplina, consultar notas, consultar boleto e pagar boletos.

![Pagina do Aluno](/prototipo-pi-imagem/2.jpg)

### Matrícula em disciplina

Área em que o aluno pode se matricular em disciplinas.

![Pagina do Aluno - Matrícula](/prototipo-pi-imagem/4.jpg)

### Consulta de Notas

Área para consulta de notas e média das disciplinas.

prototipo-pi-imagem/6.jpg(/prototipo-pi-imagem/5.jpg)

### Mensalidade 

Área que o aluno acessa para verificar boletos e realizar o pagamento.

![Mensalidade](/prototipo-pi-imagem/6.jpg)

### Área do Professor

Nessa página o professor pode escolher entre atribuir notas, criar planos de aula e registrar a frequência dos alunos.

![Área do professor](/prototipo-pi-imagem/3.jpg)

### Criar plano de Aula

Área onde professores criam planos de aula.

![Plano de aula](/prototipo-pi-imagem/7.jpg)

### Frequência de alunos

Área onde os professores registram a frequência dos alunos.

![frequência](/prototipo-pi-imagem/8.jpg)

### Área dos Fornecedores

Fornecedores podem verificar os produtos fornecidos, enviar faturas, e atualizar o cadastro.

![Área do fornecedor](/prototipo-pi-imagem/9.jpg)

### Produtos fornecidos

Área onde fornecedores tem acesso aos produtos fornecidos. Também podem adicionar novos produtos.

![produtros fornecidos](/prototipo-pi-imagem/10.jpg)

### Fatura de produtos fornecidos

Área própria para verificação de boletos de produtos fornecidos.

![boletos de produtos fornecidos](/prototipo-pi-imagem/11.jpg)

### Área para atualização cadastral dos Fornecedores

Área para atualizar as informações de cadastro dos fornecedores.

![Atualização cadastral dos fornecedores](/prototipo-pi-imagem/12.jpg)

##  Diagramas de casos de uso

#### (tentar inserir imagem se ainda tiver)

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

#### (tentar inserir imagem se ainda tiver)

### Descrição do diagrama de classes 

- Pessoa: Classe abstrata que representa uma pessoa e contém os atributos comuns a todas as subclasses,
como Nome, Endereço e Telefone;
- PessoaFisica e PessoaJuridica: Subclasses de Pessoa, representando respectivamente pessoas físicas
(alunos e professores) e pessoas jurídicas (fornecedores). PessoaFisica possui o atributo CPF, enquanto
PessoaJuridica possui o atributo CNPJ;
- Aluno e Professor: Subclasses de PessoaFisica, representando alunos e professores, respectivamente.
Ambas as classes possuem atributos específicos (Matrícula para Aluno e Registro para Professor) e um
relacionamento de associação com a classe Disciplina através do atributo Disciplinas, que é uma lista de
disciplinas;
- Fornecedor: Subclasse de PessoaJuridica, representando fornecedores. Possui um relacionamento de
agregação com a classe Produto através do atributo Produtos, que é uma lista de produtos;
- Disciplina e Produto: Classes que representam disciplinas acadêmicas e produtos, respectivamente.
Ambas possuem atributos Nome e Código.








