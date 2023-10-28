### 0 -> 1
Comando: `cat readme`
Chave: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

### 1 -> 2
Comando: `cat ./-`
Chave: rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi 

### 2 -> 3
Comando: `cat 'spaces in this filename'`
- ou: `cat "spaces in this filename"`
- ou: `cat spaces\ in\ this\ filename`
> Dica: começe a escrever o nome do arquivo e dê _TAB_.
> Ex.: cat spac`<TAB>`
Chave: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

### 3 -> 4
Comando: `cat inhere/.hidden` 
Chave: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

### 4 -> 5
Comandos:
- `cd inhere`
- `file ./-file0{0..9}` - encontra qual arquivo é um arquivo texto ASCII
- `cat ./file07` - printa a chave
Chave: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

### 5 -> 6
Comandos:
- `cd inhere`
- `find . -size 1033c -type f -exec cat {} +`
Chave: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU 

### 6 -> 7
Comando: `find . -size 33c -group bandit6 -user bandit7 -exec cat {} + 2> /dev/null`
Chave: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

### 7 -> 8
Comando: `cat data.txt | grep millionth`
Chave: TESKZC0XvTetK0S9xNwm25STk5iWrBvP

### 8 -> 9
Comando: `cat data.txt | sort | uniq -c | grep "1 "`
Chave: TESKZC0XvTetK0S9xNwm25STk5iWrBvP

### 9 -> 10
Comando: `strings data.txt | grep "=="`
Chave: G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

### 10 -> 11
Comando: `base64 -d data.txt`
Chave: 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

### 11 -> 12
Comando: `cat data.txt | tr a-z n-za-m | tr A-Z N-ZA-M`
Chave: JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

### 12 -> 13
Comando:
1. primeiro "monte" o arquivo original com `xxd -r`
2. veja seu tipo de arquivo com o comando `file`
3. renomeie para que o arquivo tenha a extensão daquele tipo de arquivo
4. vá descomprimindo/descompactando com `gzip`, `bzip2` e `tar`
5. repita 2 a 4 até conseguir um arquivo texto ASCII
Chave: wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
