# Guia Básico do ExifTool

O ExifTool é uma poderosa ferramenta de linha de comando para leitura, escrita e edição de metadados em arquivos de imagem, áudio e vídeo. Ele suporta uma ampla variedade de formatos de arquivo e é uma ferramenta essencial para qualquer pessoa investigar metadados de arquivos. Neste guia básico, vamos cobrir os comandos e operações mais comuns do ExifTool.

## Instalação

Antes de começar, você precisa instalar o ExifTool em seu sistema. Você pode encontrar as instruções de instalação em [exiftool.org](https://exiftool.org/).

## Comandos Básicos

### 1. Visualização de Metadados

Para visualizar os metadados de um arquivo, use o seguinte comando:

```shell
exiftool arquivo.extensao
```

Substitua "arquivo.extensao" pelo nome do arquivo que você deseja inspecionar. O ExifTool exibirá os metadados associados a esse arquivo.

### 2. Edição de Metadados

Para editar metadados em um arquivo, use o seguinte comando:

```shell
exiftool -tag=valor arquivo.extensao
```

Substitua "-tag" pelo nome do tag (metadado) que você deseja editar e "valor" pelo novo valor que você deseja atribuir ao tag. Novamente, substitua "arquivo.extensao" pelo nome do arquivo que você está editando.

### 3. Remoção de Metadados

Para remover um metadado específico de um arquivo, use o seguinte comando:

```shell
exiftool -tag= arquivo.extensao
```

Isso removerá o metadado especificado do arquivo. Certifique-se de incluir o sinal de igual e deixar o valor em branco para remover o tag.

### 4. Copiar Metadados de um Arquivo para Outro

Você pode copiar metadados de um arquivo para outro usando o seguinte comando:

```shell
exiftool -TagsFromFile origem.extensao destino.extensao
```

Isso copiará os metadados do arquivo de origem para o arquivo de destino.

## Exemplos Adicionais

Aqui estão alguns exemplos adicionais de uso do ExifTool:

- Exibir todos os metadados de um arquivo em formato JSON:

```shell
exiftool -json arquivo.extensao
```

- Renomear um arquivo com base em seus metadados:

```shell
exiftool "-FileName<CreateDate" -d "%Y%m%d_%H%M%S%%-c.%%e" arquivo.extensao
```

Este comando renomeia o arquivo com base na data de criação.

## Conclusão

Este é apenas um guia básico para começar com o ExifTool. Ele oferece muitos recursos avançados para manipulação de metadados, como a edição em lote e a criação de scripts personalizados. Consulte a documentação oficial do ExifTool para obter mais informações e opções avançadas: [exiftool.org](https://exiftool.org/).

Lembre-se sempre de fazer backup de seus arquivos antes de editar metadados, pois as alterações podem ser irreversíveis.
