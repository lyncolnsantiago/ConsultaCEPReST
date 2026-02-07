# Consulta_CEP_REST 📍

O **ConsultaCEPREST** é uma aplicação console desenvolvida em **Java** para automatizar a busca de endereços através do consumo da API REST do **ViaCEP**. O sistema permite que o usuário informe um CEP e obtenha instantaneamente os dados de localização formatados no terminal.

---

### 🛠 Tecnologias e Dependências

O projeto foi construído utilizando as seguintes tecnologias:

* **Java 25**: Versão mais recente da linguagem para desenvolvimento robusto.
* **Maven 3.9.11**: Gerenciador de dependências e automação de build.
* **Apache HttpClient (Fluent-HC)**: Biblioteca para realizar requisições HTTP de forma simplificada.
* **Google Gson**: Ferramenta para conversão de dados JSON em objetos Java (POJOs).

---

### ✨ Funcionalidades Principais

* **Consumo de API Externa**: Realiza chamadas assíncronas ao serviço ViaCEP para recuperar informações de endereço.
* **Tratamento de Erros Personalizado**: Implementação da exceção `CEPNotFoundException` para lidar com CEPs inexistentes na base de dados.
* **Mapeamento de Dados Completo**: A classe `Endereco` suporta todos os campos retornados pela API, como logradouro, bairro, localidade, UF e códigos regionais (IBGE, GIA, etc.).
* **Interface via Terminal**: Interação simples com o usuário utilizando a classe `Scanner`.

---

### 📂 Estrutura do Projeto

A arquitetura do código está organizada nos seguintes pacotes:

1.  **`br.com.senai.s042`**: Contém a classe principal `Application` que inicia o programa.
2.  **`br.com.senai.s042.client`**: Responsável pela lógica da classe `ViaCEPClient`, que gerencia a comunicação HTTP.
3.  **`br.com.senai.s042.model`**: Contém a classe `Endereco`, mapeada para receber o JSON da API.
4.  **`br.com.senai.s042.exception`**: Local onde as exceções customizadas do sistema são definidas.
---

### 🚀 Como Executar

1.  **Pré-requisitos**: Ter o **JDK 25** e o **Maven** configurados em sua máquina.
2.  **Clone o repositório**:
    ```bash
    git clone [https://github.com/seu-usuario/ConsultaCEPREST.git](https://github.com/seu-usuario/ConsultaCEPREST.git)
    ```
3.  **Compile o projeto**:
    ```bash
    mvn clean install
    ```
4.  **Rode a aplicação**: Execute a classe `Application.java` através da sua IDE (IntelliJ) ou via linha de comando.

---

### 👨‍💻 Autor

Desenvolvido por **Lyncoln** em aula.
