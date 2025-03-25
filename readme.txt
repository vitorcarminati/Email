E-mail 1: Processamento Assíncrono com XMLHttpRequest

Assunto:  Implementação do Fluxo Assíncrono (XMLHttpRequest)

Olá, equipe!

Vamos implementar o XMLHttpRequest para requisições assíncronas no e-commerce. Segue o fluxo resumido:

 Ciclo da Requisição:

**Inicialização:**
**javascript**

const xhr = new XMLHttpRequest();

**Configuração:**
**javascript**

xhr.open('GET', 'https://api.wjvcg.com/produtos', true); // true = assíncrono
xhr.setRequestHeader('Content-Type', 'application/json');

**Tratamento da Resposta:**
**javascript**

xhr.onload = function() {
  if (xhr.status === 200) {
    const response = JSON.parse(xhr.responseText);
    console.log("Dados recebidos:", response);
    // Atualize a UI aqui!
  } else {
    console.error("Erro na requisição:", xhr.statusText);
  }
};

**Tratamento de Erros:**
**javascript**

xhr.onerror = function() {
  console.error("Falha na conexão");
};

**Envio:**
**javascript**

xhr.send();

** Benefícios:**
 Zero bloqueio de UI (usuário continua navegando)
 Eficiência (só carrega dados necessários)
 Performance (melhor experiência)

Qualquer dúvida, estou à disposição!

Abraços,









E-mail 2: Fluxo Colaborativo no GitHub

Assunto:  GitHub - Como Contribuir no Projeto

Time,

Vamos trabalhar de forma colaborativa! Siga esses passos:

**Configuração Inicial:
Clone o repositório:**

git clone https://github.com/vitorcarminati/Email.git

**Configure seu Git:**

git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

** Fluxo de Trabalho:
Crie uma branch para sua tarefa:

git checkout -b feature/sua-feature

**Faça e envie as alterações:**

git add .
git commit -m "Adiciona filtro de produtos"
git push origin feature/sua-feature

**Abra um Pull Request no GitHub para revisão.**
** Repositório:** github.com/vitorcarminati/Email.git

**Importante:**
Sempre dê **git pull antes de começar.
Mensagens de commit claras e objetivas.
Revise o código dos colegas.

Vamos construir algo incrível juntos! 

Abraços.