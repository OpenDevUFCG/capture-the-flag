Claro, aqui está uma versão mais curta do guia Nmap em formato Markdown:

# Guia Básico do Nmap

O Nmap é uma ferramenta de código aberto para descobrir informações sobre redes e dispositivos. Abaixo estão alguns comandos básicos.

## Instalação

- Linux: Use o gerenciador de pacotes ou baixe no [site oficial](https://nmap.org/download.html).

## Comandos Básicos

### Scan de Host Único

```shell
$ nmap <alvo>
```

### Scan de Intervalo de IPs

```shell
$ nmap <início>-<fim>
```

### Scan de Portas Específicas

```shell
$ nmap -p <portas> <alvo>
```

### Identificar Serviços e Versões

```shell
$ nmap -sV <alvo>
```

### Scan Agressivo

```shell
$ nmap -A <alvo>
```

Lembre-se de obter autorização para escanear redes ou hosts que não sejam de sua propriedade.