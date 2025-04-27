
# Guia para Criar uma Instância Gerenciada de SQL no Azure

Este guia é destinado a iniciantes e fornecerá um passo a passo detalhado para a criação de uma **Instância Gerenciada de SQL no Azure**. A Instância Gerenciada de SQL é um serviço de banco de dados totalmente gerenciado pela Microsoft, proporcionando escalabilidade, segurança e alta disponibilidade.

## 📌 Pré-requisitos

Antes de iniciar, certifique-se de que possui:
- 🔹 **Conta do Azure**: Se não tiver, [crie uma conta gratuita](https://azure.microsoft.com/pt-br/free/).
- 🔹 **Assinatura do Azure ativa**: Pode ser um plano pago ou a versão gratuita.
- 🔹 **Grupo de Recursos**: Uma coleção lógica de recursos do Azure.

## 🔹 Passo 1: Acessar o Portal do Azure

1. Acesse o [Portal do Azure](https://portal.azure.com).
2. Faça login com sua conta do Azure.
3. No painel de controle, clique em **"Criar um recurso"**.

## 🔹 Passo 2: Criar a Instância Gerenciada de SQL

1. Na barra de pesquisa, digite **"Instância Gerenciada de SQL"** e selecione o serviço correspondente.
2. Clique em **"Criar"** para iniciar o processo de configuração.

## 🔹 Passo 3: Configurar a Instância

Aqui, você definirá detalhes essenciais para sua instância.

### 🏗️ Configuração Básica:
- **Assinatura**: Escolha a assinatura do Azure que será usada.
- **Grupo de Recursos**: Escolha um existente ou crie um novo.
- **Nome da Instância**: Escolha um nome único para identificação.
- **Região**: Selecione uma região próxima para melhor latência.
- **Versão do SQL Server**: Escolha a versão desejada para compatibilidade.

### 💰 Configuração de Preço:
- Escolha entre as **camadas de serviço**, como:
  - **General Purpose** (para cargas de trabalho moderadas)
  - **Business Critical** (para desempenho e alta disponibilidade)
  - **Hyperscale** (para bancos de dados muito grandes)

### 🔐 Configuração de Autenticação:
1. Defina um **usuário administrador** e uma **senha segura**.
2. Escolha o tipo de autenticação (Azure AD ou SQL Authentication).

### ⚙️ Configurações Adicionais:
- **Backup e Recuperação**: Configure backups automáticos.
- **Conectividade**: Escolha entre **rede pública** ou **privada** para segurança.

## 🔹 Passo 4: Revisar e Criar

1. Revise todas as configurações definidas.
2. Clique em **"Criar"** e aguarde a implantação (pode levar alguns minutos).

## 🔹 Passo 5: Conectar-se à Instância

Após a criação:
1. Vá até o recurso da **Instância Gerenciada de SQL** no portal do Azure.
2. No painel da instância, copie a **String de Conexão**.
3. Utilize um cliente SQL, como:
   - **SQL Server Management Studio (SSMS)** 
   - **Azure Data Studio**
   - **Aplicações personalizadas via conexão JDBC ou ODBC**

## 🔹 Passo 6: Teste a Conexão

1. Abra o **SSMS** e insira a **String de Conexão**.
2. Faça login com o usuário e senha configurados.
3. Execute um comando SQL para validar:
   ```sql
   SELECT @@VERSION;
   ```
Se tudo estiver correto, sua instância estará pronta para uso! ✅

## 📖 Fontes

[criar Instância Gerenciada de SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal)

[Configurando o Azure SQL Database](https://youtu.be/CIzs7KY3Jl4?si=w8TpSJGJHArQzrgY)

   
