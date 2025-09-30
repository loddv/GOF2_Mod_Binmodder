# binmodder

Programa Python para substituir strings nos arquivos `.bin` do Galaxy On Fire 2. Também utiliza uma versão do random-googletrans e a ferramenta gof2translate.

**Feito para o Mod GOF2 Google Translate**

## Dependências

- O `gof2translate.py` utiliza o googletrans 3.1.0a0 para evitar o erro AttributeError: 'NoneType' object has no attribute 'group'.
- Você precisa instalar esta versão específica do pacote:

```bash
pip install googletrans==3.1.0a0
```

## Como usar

### 1. Interface Gráfica (GUI)

Execute o arquivo `binModderGui.py`:

```bash
python binModderGui.py
```

Ou baixe um dos executáveis na seção de [releases](https://github.com/loddv/GOF2_Mod_Binmodder/releases/) e rode o `binModderGui.exe`.

- Selecione o arquivo `.bin` que deseja modificar clicando em "Choose .bin file".

#### Usando arquivos .txt

- Crie um arquivo `.txt` contendo as strings presentes no arquivo `.bin` que você deseja substituir (você pode visualizar essas strings em um editor hexadecimal), separando cada string por uma nova linha.
- Importe esse arquivo `.txt` no binmodder clicando em "Choose strings to be replaced".
- Se quiser escolher os substitutos manualmente, crie outro `.txt` com as strings de substituição (na mesma ordem), separadas por nova linha, e importe clicando em "Choose replacement strings".

#### Usando o recurso random-googletrans

- Ao utilizar o `gof2translate`, quaisquer arquivos `.txt` importados como substituição serão ignorados.
- Para usar esse recurso, marque a caixa "gof2translate" e clique em "Replace".

#### Importando strings automaticamente

- O binmodder pode usar o [gofdetect](https://github.com/loddv/gof2detect), que extrai automaticamente todas as strings dos arquivos `.bin`.
- Para usar, selecione um arquivo `.bin` e clique em "detect". Depois, escolha o tipo de arquivo `.bin` que está modificando.

### 2. Linha de Comando

Você pode executar o script principal diretamente pelo terminal:

```bash
python binmodder.py
```

Siga as instruções exibidas no terminal para processar os arquivos `.bin` conforme necessário.

## Mod GOF2 Google Translate

Confira a página do mod:  
[GOF2 Google Translated (ainda não finalizado) no Mod DB](https://www.moddb.com/mods/gof2-google-translated)