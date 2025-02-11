# Prompt-de-Comando

***

## Explicação dos comandos Batch
Um arquivo batch é um arquivo de texto simples contendo uma sequência de comandos que são interpretados e executados pelo Prompt de Comando do Windows (**CMD**). A principal característica dos arquivos batch é que eles permitem que você automatize processos ou tarefas, como copiar arquivos, mover pastas, executar programas, fazer verificações, entre outros.


![Descrição da Imagem](https://www.ionos.com/pt-br/digitalguide/fileadmin/DigitalGuide/Screenshots_2020/batch-file-in-windows-explorer.jpg)

## Principais Comandos Usados em Arquivos Batch

- ECHO: Escreve na tela
```
ECHO Olá, Mundo!
```
- ECHO OFF: Oculta informações e o código executado pelo sistema.
```
@ECHO OFF
ECHO Este é um exemplo sem exibir comandos.
```
- ECHO ON: Exibe informações e o código executado pelo sistema.
```
ECHO ON
ECHO Este comando exibirá todos os comandos executados no console.
```
- ECHO.: Salta uma linha.
```
ECHO Linha 1
ECHO.
ECHO Linha 2
```
- @ECHO: Faz com que o prompt fique oculto durante toda execução.
```
Linha 1

Linha 2
````
- SET: Cria variável que pode ser referenciada através de %variável%.
```
SET nome=João
ECHO Olá, %nome%!
```
- CLS: Limpa o console.
```
CLS
ECHO Console limpo.
```
- IF e ELSE: Estruturas condicionais.
```
SET idade=18
IF %idade% GEQ 18 (
    ECHO Você é maior de idade.
) ELSE (
    ECHO Você é menor de idade.
)
```
- GOTO: Avança até determinado trecho do lote.
```
@ECHO OFF
ECHO Início do script
GOTO Fim

:Estrutura
ECHO Este trecho nunca será executado.

:Fim
ECHO Fim do script
```
- FOR: Estrutura de repetição.
```
FOR %%i IN (1 2 3 4 5) DO (
    ECHO Número %%i
)
```
- PAUSE: Faz uma pausa, e exibe: “Pressione qualquer tecla para continuar.”
```
ECHO Este é o início do script.
PAUSE
ECHO O script continuará após pressionar uma tecla.
```
- REM: Utilizado para fazer comentários.
```
REM Este é um comentário.
ECHO Este comando será executado.
```
- START: Inicializa um aplicativo ou programa.
```
START calc.exe
```
- MOVE: Move (recorta) um arquivo de um diretório para outro.
```
MOVE C:\origem\arquivo.txt D:\destino\
```


