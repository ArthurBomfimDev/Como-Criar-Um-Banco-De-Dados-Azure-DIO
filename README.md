<div align="center">
<br>
<h1>💾 Como Criar um Banco de Dados SQL na Azure - Desafio DIO</h1>
</div>

📝 Sobre o que se trata este repositório?
Este repositório contém um guia completo e visual para a criação de uma instância de Banco de Dados SQL no Microsoft Azure, como parte do desafio de projeto do Bootcamp .NET, C#, Docker e Azure oferecido pela DIO.

O objetivo deste documento é registrar o passo a passo da criação do banco de dados, aplicando na prática os conhecimentos sobre serviços de nuvem e documentando a experiência.

<div align="center">
<img src="https://hermes.digitalinnovation.one/assets/diome/logo.png" width="250" alt="Logo DIO">
<img src="https://upload.wikimedia.org/wikipedia/commons/a/a8/Microsoft_Azure_Logo.svg" width="300" alt="Logo Azure">
</div>

---

# 🚀 Passo a Passo para Criar seu Banco de Dados no Azure
Siga as etapas detalhadas abaixo para provisionar e configurar sua instância do Banco de Dados SQL.

# 1️⃣ Acessando o Portal do Azure e Iniciando a Criação
Acesse o Portal: Primeiro, faça login no portal do Azure.

Localize o serviço: Na barra de busca ou no menu lateral, procure por "Bases de dados SQL" e clique para aceder.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco1.png" alt="Tela inicial do portal do Azure, destacando a opção Bases de dados SQL.">

Inicie a Criação: Na página "Bases de dados SQL", clique no botão "+ Criar" para começar a configuração.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco2.png" alt="Tela de gerenciamento de bases de dados, destacando o botão para criar uma nova.">

# 2️⃣ Configurando as Informações Básicas
Esta é a etapa principal, onde definimos todas as características do nosso banco de dados e do servidor que o irá hospedar.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco3.png" alt="Tela inicial de configuração da base de dados.">

Detalhes do Servidor
Antes de criar a base de dados, precisamos de um servidor para a alojar. Clique em "Criar novo" na opção "Servidor".
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco4.png" alt="Tela para criar um novo servidor.">

Aqui, definimos as credenciais de acesso e a localização do servidor.

Nome do servidor: Um nome único globalmente.

Localização: A região onde o servidor ficará.

Método de autenticação: Escolhi "Utilizar a autenticação apenas do Microsoft Entra" para uma gestão de identidade mais moderna e segura, mas a autenticação SQL com utilizador e palavra-passe também é uma opção válida.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco5.png" alt="Configuração do nome, localização e autenticação do servidor.">

Detalhes da Base de Dados
Com o servidor criado, voltamos para a tela principal para finalizar a configuração.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco6.png" alt="Tela de configuração da base de dados com o servidor já selecionado.">

Ambiente de carga de trabalho: Selecionei "Desenvolvimento". Esta opção ajusta as configurações de desempenho e custo para um ambiente de estudo, sendo a mais económica.

Redundância de armazenamento de cópias de segurança: Optei por "Armazenamento de cópia de segurança localmente redundante". Para um laboratório, esta é a opção mais barata e suficiente, pois cria cópias de segurança dentro do mesmo datacenter.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco7.png" alt="Configuração do ambiente e da redundância.">

# 3️⃣ Configurando a Rede
Nesta etapa, definimos como iremos aceder ao nosso banco de dados.

Método de conectividade: Escolhi "Ponto final público" para permitir o acesso a partir da minha máquina local.

Regras de firewall: Marquei "Adicionar o endereço IP do cliente atual" como Sim. Este passo é essencial, pois autoriza o meu computador a ligar-se ao banco de dados.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco8.png" alt="Configuração da rede e das regras de firewall.">

# 4️⃣ Revisão e Criação
Após passar pelas abas de "Segurança", "Definições adicionais" e "Sinalizadores" (onde mantive as predefinições), chegamos à tela de revisão.

O Azure faz uma validação final. Se tudo estiver correto, a mensagem "Validação bem-sucedida" será exibida.

Confira o resumo de todas as configurações e clique em "Criar".
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco9.png" alt="Tela de revisão final com a validação bem-sucedida.">

# 5️⃣ Implantação Concluída
Aguarde alguns minutos enquanto o Azure provisiona todos os recursos.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco10.png" alt="Tela mostrando o progresso da implantação.">

Quando o processo for finalizado, você verá a tela de confirmação: "A sua implantação está concluída".

Clique em "Ir para o recurso" para ver o painel de controlo do seu novo banco de dados.
<img src="https://raw.githubusercontent.com/ArthurBomfimDev/Como-Criar-Um-Banco-De-Dados-Azure-DIO/main/imagens/banco11.png" alt="Tela de sucesso mostrando que a implantação foi concluída.">

---

# 🎯 Para mim:
Concluir este laboratório sobre o Banco de Dados SQL do Azure foi uma experiência muito enriquecedora. Entender na prática como configurar um servidor, definir regras de acesso e escolher as opções de custo e desempenho é crucial para qualquer desenvolvedor que queira construir aplicações robustas na nuvem.

Este conhecimento prático complementa a teoria e me dá mais confiança para desenhar e implementar soluções completas, pensando não apenas no código, mas em toda a infraestrutura de dados que o suporta.
