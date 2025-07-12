<h2>📘 Projeto: Banco Digital com Spring Boot</h2>

<h3>🧾 Descrição</h3>
<p>Este é um projeto de <strong>API REST para um banco digital</strong>, desenvolvido com Spring Boot, que permite operações como:</p>
<ul>
  <li>Cadastro de clientes</li>
  <li>Criação e gerenciamento de contas (corrente e poupança)</li>
  <li>Emissão de cartões (crédito e débito)</li>
  <li>Realização de transações (saque, depósito, transferência, Pix)</li>
  <li>Contratação e cancelamento de seguros</li>
</ul>

<hr>

<h3>🛠️ Tecnologias Utilizadas</h3>
<ul>
  <li>Java 17+</li>
  <li>Spring Boot</li>
  <li>Spring Data JPA</li>
  <li>H2 Database</li>
  <li>Postman (para testes de API)</li>
  <li>Maven</li>
</ul>

<hr>

<h3>🔧 Como executar o projeto</h3>
<ol>
  <li>Clone o repositório:
    <pre><code>git clone https://github.com/seu-usuario/banco-digital-springboot.git</code></pre>
  </li>
  <li>Abra no Eclipse, IntelliJ ou VS Code</li>
  <li>Execute a classe <strong>BancoDigitalJpaApplication.java</strong></li>
  <li>JDBC URL: <strong>jdbc:h2:mem:testdb</strong></li>
  <li>Usuário: <strong>sa</strong> / Senha: (em branco)</li>
</ol>

<hr>

<h3>📮 Testes com Postman</h3>
<p>Você pode testar todos os endpoints usando o Postman. Algumas rotas disponíveis:</p>

<table>
  <thead>
    <tr>
      <th>Método</th>
      <th>Endpoint</th>
      <th>Descrição</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>POST</td>
      <td>/cliente/add</td>
      <td>Adiciona novo cliente</td>
    </tr>
    <tr>
      <td>POST</td>
      <td>/conta/criar</td>
      <td>Cria uma nova conta</td>
    </tr>
    <tr>
      <td>GET</td>
      <td>/conta/detalhes/{id}</td>
      <td>Detalha uma conta</td>
    </tr>
    <tr>
      <td>POST</td>
      <td>/conta/{id}/pix</td>
      <td>Realiza uma transferência via Pix</td>
    </tr>
    <tr>
      <td>POST</td>
      <td>/cartao/emitir</td>
      <td>Emite um cartão (crédito ou débito)</td>
    </tr>
    <tr>
      <td>POST</td>
      <td>/cartao/{id}/pagamento</td>
      <td>Realiza um pagamento com cartão</td>
    </tr>
    <tr>
      <td>POST</td>
      <td>/seguro/cartao/{id}</td>
      <td>Contrata um seguro</td>
    </tr>
    <tr>
      <td>DELETE</td>
      <td>/seguro/{id}/cancelar</td>
      <td>Cancela um seguro</td>
    </tr>
  </tbody>
</table>

<h3>📦 Coleção Postman</h3>
<p>Você pode importar a coleção de testes diretamente no Postman:</p>

👉 [Clique aqui para baixar a coleção do Postman](https://github.com/anacristinademoura/banco-digital-jpa/blob/master/docs/banco-digital-collection.json)

Ou acesse o arquivo dentro da pasta `/docs/banco-digital-collection.json`.

<hr>

<h3>🧠 Conceitos Aplicados</h3>
<ul>
  <li>Princípio da Responsabilidade Única (SRP)</li>
  <li>Camada de DTO para segurança e clareza</li>
  <li>Validações robustas com exceções personalizadas</li>
  <li>Uso de anotações JPA (<code>@OneToOne</code>, <code>@ManyToOne</code>, etc.)</li>
  <li>Tratamento de erros com <code>try-catch</code> nos controllers</li>
</ul>

<hr>

<h3>💡 Possíveis Melhorias Futuras</h3>
<ul>
  <li>Persistência em banco real (PostgreSQL, MySQL)</li>
  <li>Autenticação com Spring Security</li>
  <li>Documentação automática com Swagger</li>
  <li>Testes automatizados com JUnit e Mockito</li>
</ul>

<hr>

<h3>🙋‍♀️ Autora</h3>
<p><strong>Ana Cristina de Moura Santana</strong></p>
<p>Estudante de Análise e Desenvolvimento de Sistemas</p>
<p><a href="https://www.linkedin.com/in/anacristinadmoura/" target="_blank">LinkedIn</a></p>

<hr>
