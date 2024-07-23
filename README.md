# Servidor Minecraft Cross 

**Documentação: Criação de um Servidor Multplataforma Minecraft com PaperMC e Geyser/Floodgate**

Este documento descreve como configurar um servidor multplataforma Minecraft usando o PaperMC e os plugins GeyserMC e Floodgate, baseado no arquivo de instruções fornecido.

**Pré-requisitos:**

- Um computador com acesso à internet e espaço livre em disco suficiente para armazenar o servidor e plugins.
- Java Development Kit (JDK) 8 ou superior instalado.
- Editor de texto para edição de arquivos.

**Passo 1: Baixar o Servidor PaperMC**

1. Acesse o site do PaperMC: https://papermc.io/downloads/all
2. Baixe a versão mais recente do PaperMC para o seu sistema operacional.
3. Extraia o conteúdo do arquivo baixado para uma pasta de sua preferência.

**Passo 2: Baixar GeyserMC e Floodgate**

1. Acesse o site do GeyserMC: https://geysermc.org/download/
2. Baixe os arquivos JAR do GeyserMC e Floodgate.
3. Crie uma pasta chamada `plugins` dentro da pasta do seu servidor PaperMC.
4. Copie os arquivos JAR do GeyserMC e Floodgate para a pasta `plugins`.

**Passo 3: Iniciar o Servidor**

1. Abra um terminal ou prompt de comando na pasta do seu servidor PaperMC.
2. Execute o comando a seguir para iniciar o servidor:

```
java -Xmx4G -Xms4G -jar paper-XXXXX --nogui
```

Substitua `paper-XXXXX` pelo nome do arquivo JAR do PaperMC que você baixou.

**Passo 4: Aceitar os Termos**

1. Abra o arquivo `eula.txt` na pasta do seu servidor PaperMC com um editor de texto.
2. Altere a linha `eula=false` para `eula=true`.
3. Salve e feche o arquivo.

**Passo 5: Copiar a Chave Floodgate**

1. Acesse a pasta `plugins/floodgate` no seu servidor PaperMC.
2. Copie o arquivo `key.pem` para a pasta `plugins/Geyser-Spigot`.

**Passo 6: Reiniciar o Servidor**

1. No terminal ou prompt de comando, pare o servidor usando o comando `CTRL + C`.
2. Execute novamente o comando de inicialização do servidor do Passo 3.

**Passo 7: Testar a Conexão**

1. Abra o cliente Minecraft e conecte-se ao seu servidor usando o endereço IP do seu computador e a porta padrão (25565).
2. Se você vir o GeyserMC conectando-se ao servidor e os jogadores podem se conectar sem problemas, a configuração foi bem-sucedida.

**Notas:**

- Certifique-se de que a porta 25565 esteja aberta em seu firewall e não esteja sendo bloqueada por outros aplicativos.
- Se você estiver usando um VPS ou outro provedor de hospedagem, verifique as configurações de rede e firewall fornecidas pelo provedor.
- Para obter mais informações sobre a configuração e otimização do seu servidor, consulte a documentação oficial do PaperMC, GeyserMC e Floodgate.