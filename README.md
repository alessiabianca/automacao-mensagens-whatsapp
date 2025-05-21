# automa-o-mensagens-whatsapp
Descrição:
Este projeto utiliza a biblioteca Selenium para automatizar o envio de mensagens e arquivos via WhatsApp Web. O código lê dados de uma planilha Excel, personaliza as mensagens e envia para os contatos listados, podendo também anexar arquivos quando necessário.

Pré-requisitos:
Python 3.x instalado

Bibliotecas Python: selenium, pandas, urllib, time, os

Navegador Chrome e o driver correspondente (ChromeDriver) configurado

Acesso ao WhatsApp Web (https://web.whatsapp.com)

Instalação:
Clone o repositório ou baixe o arquivo Envio Whatsapp.ipynb.

Instale as dependências executando:

bash
pip install selenium pandas openpyxl
Certifique-se de que o ChromeDriver está no PATH ou especifique seu caminho no código.

Configuração
Prepare uma planilha Excel chamada Envios.xlsx com as seguintes colunas:

nome: Nome do contato (usado para personalizar a mensagem).

mensagem: Texto da mensagem, onde "fulano" será substituído pelo nome do contato.

arquivo: Nome do arquivo a ser enviado (use "N" para não enviar arquivo).

telefone: Número de telefone no formato internacional (ex: +5511999999999).

Coloque os arquivos a serem enviados na pasta arquivos/.

Uso
Execute o Jupyter Notebook Envio Whatsapp.ipynb.

O script irá:

Abrir o WhatsApp Web no navegador Chrome.

Aguardar que você faça login manualmente (leia o QR code).

Ler os dados da planilha Envios.xlsx.

Enviar as mensagens personalizadas para cada contato.

Anexar arquivos quando especificado.

Observações
O WhatsApp Web deve permanecer aberto e logado durante a execução.

O script inclui pausas (time.sleep) para garantir o carregamento adequado das páginas.

Números inválidos são automaticamente detectados e ignorados.

Personalize os caminhos e XPaths conforme necessário para sua versão do WhatsApp Web.
