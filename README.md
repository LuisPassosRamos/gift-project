### **README.md** – GiftList

---

## 📋 **Descrição do Projeto**

**GiftList** é uma plataforma que permite a criação e compartilhamento de **listas de presentes e desejos** para eventos como aniversários, casamentos, chá de bebê, ou até para organização pessoal. Com recursos sociais integrados, como perfis públicos/privados e interações entre usuários, o projeto busca facilitar a comunicação entre anfitriões e convidados. Os convidados podem marcar itens como “reservados”, evitando duplicidades e proporcionando uma experiência mais personalizada na escolha dos presentes.

### **Funcionalidades Principais**  
- Criação de **listas de presentes** públicas e privadas.
- Possibilidade de marcar presentes como escolhidos.
- Perfis sociais com informações sobre preferências e gostos.
- Interações sociais, como “lembrei de você” e sugestões anônimas.
- Opções de compra física ou virtual, além de doação financeira.
- **Autenticação social** via Google/Facebook e notificações por e-mail.

---

## 🛠 **Tecnologias Utilizadas**
- **Backend**: Spring Boot, JPA, MySQL, Spring Security, Spring Mail, Flyway  
- **Frontend**: React.js, Axios, Material UI / TailwindCSS  

---

## 📝 **To-Do List Geral**  

### **Backend**
1. **Configuração do Projeto**  
   - [ ] Inicializar o projeto no Spring Boot com Java 17.  
   - [ ] Configurar dependências: Web, Data JPA, MySQL Driver, Security, OAuth2, Mail e Validation.  
   - [ ] Criar estrutura inicial do banco de dados com **Flyway**.  
   - [ ] Configurar autenticação (OAuth2) para login social (Google/Facebook).  

2. **Modelagem e Persistência**  
   - [ ] Implementar entidades principais: `Usuario`, `Lista`, `ItemLista`, `Evento`.  
   - [ ] Implementar as relações entre entidades (ex.: `Usuario` pode ter várias `Listas`).  
   - [ ] Configurar repositórios JPA para persistência.  

3. **Funcionalidades de API**  
   - [ ] Criar endpoints REST para **CRUD de listas e itens**.  
   - [ ] Implementar filtros e busca por listas públicas.  
   - [ ] Expor API para controle de reserva de itens.  
   - [ ] Criar funcionalidade de "Lembrei de Você" via API.  

4. **Segurança e Validações**  
   - [ ] Implementar autenticação e autorização com Spring Security.  
   - [ ] Configurar regras de visibilidade de perfis e listas.  
   - [ ] Validar dados com Bean Validation (ex.: nomes, e-mails).

5. **Envio de Notificações e E-mails**  
   - [ ] Configurar envio de notificações de reserva via Spring Mail.  
   - [ ] Implementar envio de e-mails com confirmação de presentes.

---

### **Frontend**
1. **Setup do Projeto**  
   - [ ] Inicializar projeto com React.js.  
   - [ ] Configurar roteamento (React Router) para navegação entre páginas.  
   - [ ] Integrar Axios para consumo da API REST.  

2. **Interface de Usuário (UI/UX)**  
   - [ ] Criar telas de login e registro (incluindo login social).  
   - [ ] Implementar dashboard do usuário com perfis e listas.  
   - [ ] Criar formulário dinâmico para criação e edição de listas.  
   - [ ] Implementar a funcionalidade de reserva de itens com feedback visual.  

3. **Funcionalidades de Interação**  
   - [ ] Adicionar sistema de busca e filtros para perfis e listas públicas.  
   - [ ] Implementar notificações de reserva e ações sociais ("Lembrei de Você").  
   - [ ] Exibir histórico de presentes e status das listas.  

4. **Estilização e Layout**  
   - [ ] Aplicar design responsivo com **Material UI / TailwindCSS**.  
   - [ ] Ajustar para acessibilidade (a11y).  

---

## 🚀 **Execução e Deploy**
### **Backend**
1. Execute o banco de dados MySQL localmente ou via Docker.  
2. Configure as credenciais do banco e OAuth2 em `application.yml`.  
3. Execute o projeto com:  
   ```bash
   ./mvnw spring-boot:run
   ```

### **Frontend**
1. Instale as dependências:  
   ```bash
   npm install
   ```  
2. Execute o projeto React:  
   ```bash
   npm start
   ```

---

## 📚 **Contribuição**
1. Faça um fork do projeto.
2. Crie uma nova branch: `git checkout -b minha-nova-feature`.
3. Commit suas mudanças: `git commit -m 'Minha nova feature'`.
4. Envie para a branch principal: `git push origin minha-nova-feature`.
5. Crie um Pull Request.

---

## 📦 **Licença**
Este projeto está licenciado sob a [MIT License](https://opensource.org/licenses/MIT).

---

## 💬 **Contato**
Se você tiver dúvidas ou sugestões, entre em contato por meio do meu [GitHub](https://github.com/seuusuario) ou [LinkedIn](https://www.linkedin.com/in/seuusuario).

---

Com esse **README.md**, seu projeto terá uma documentação inicial organizada, clara para colaboradores, e fácil de expandir à medida que novas funcionalidades forem adicionadas.
