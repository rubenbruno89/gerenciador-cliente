# Gerenciador de Clientes IPTV

Aplicação web em HTML, CSS e JavaScript para cadastrar clientes, acompanhar vencimentos, preparar mensagens de WhatsApp, configurar pagamentos via PIX e criar backups locais.

## Acessar o site

- [Abrir pelo ShardWeb](https://gc-pro.shardweb.app/)
- [Abrir pelo GitHub Pages](https://rubenbruno89.github.io/gerenciador-cliente/)

## Funcionalidades

- Cadastro, edição e exclusão de clientes.
- Controle de status e datas de vencimento.
- Busca, filtros e ordenação da lista de clientes.
- Indicadores de clientes ativos, vencidos e próximos do vencimento.
- Modelos de mensagens para WhatsApp sem emojis no texto enviado.
- Abertura da conversa do cliente no WhatsApp para revisar e enviar a mensagem.
- Configuração de chave PIX, tipo de chave, recebedor, cidade e valor padrão.
- Geração local do código PIX copia e cola.
- Exportação de backups nos formatos `.json`, `.db` e `.bd`.
- Exportação de uma planilha `.csv`.
- Importação de backups e opção para substituir ou mesclar os clientes.

## Como usar

1. Acesse um dos links acima ou abra o arquivo HTML no navegador.
2. Abra **Configurações** para informar o nome da loja e, se desejar, os dados do PIX.
3. Use **Cliente** para cadastrar os dados de cada cliente.
4. Use os botões da tabela para editar, renovar, gerar PIX ou preparar uma mensagem de WhatsApp.
5. Acesse **Backup** e escolha **Exportar** para salvar uma cópia ou **Importar** para restaurar um arquivo.

## Armazenamento e backups

Os dados do painel são armazenados no `localStorage` do navegador. O aplicativo não usa um servidor próprio nem sincroniza os dados automaticamente com a nuvem.

**Os arquivos `.db` e `.bd` são backups em formato JSON com outra extensão; não são bancos de dados SQLite.** O formato `.csv` é destinado a planilhas e não pode ser importado pelo painel. Para restaurar os dados, use um backup `.json`, `.db` ou `.bd`.

Os dados armazenados dependem do navegador e do endereço do site. Por isso, os dois links acima podem ter dados separados. Para transferir os clientes de um endereço para o outro, exporte um backup no primeiro e importe-o no segundo.

Faça backups periódicos e mantenha uma cópia em local seguro.

## Privacidade e segurança

Os dados são guardados localmente no navegador. Backups podem conter nomes, telefones, usuários, senhas, informações de pagamento e chave PIX. Eles não são criptografados pelo aplicativo: proteja os arquivos e não os compartilhe publicamente.

O WhatsApp é aberto para que você confira e envie a mensagem. O aplicativo não envia mensagens automaticamente nem confirma pagamentos.

## Tecnologias

- HTML
- CSS
- JavaScript
- `localStorage` do navegador

Não é necessário instalar dependências ou executar um processo de compilação.

## Uso responsável

Este projeto é uma ferramenta de organização de clientes. Use-o somente para administrar serviços e conteúdos que você está autorizado a oferecer.
