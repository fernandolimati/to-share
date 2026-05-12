# Em.Edith.2.zip — Partes

Este diretório contém o asset `Em.Edith.2.zip` do release [1.0](https://github.com/fernandolimati/to-share/releases/tag/1.0) (~482 MB) dividido em 33 partes binárias de 15 MB cada (a última com ~2,4 MB), porque o arquivo original ultrapassa o limite de 100 MB por arquivo do GitHub.

## Como reconstruir o arquivo original

### Linux / macOS

```bash
cat Em.Edith.2.zip.part-* > Em.Edith.2.zip
```

### Windows (PowerShell)

```powershell
Get-Content Em.Edith.2.zip.part-* -Raw -Encoding Byte | Set-Content Em.Edith.2.zip -Encoding Byte
```

### Windows (cmd)

```cmd
copy /b Em.Edith.2.zip.part-* Em.Edith.2.zip
```

## Verificação de integridade

Após a reconstrução, valide o SHA-256:

```bash
sha256sum Em.Edith.2.zip
```

Esperado:

```
77e2ff481e2aa77fb51680e9cd13ac17240f2a8b33773a53651b39ced73f009e  Em.Edith.2.zip
```

## Conteúdo do zip

```
Em Edith/tokenizer.json.html   (351 KB)
Em Edith/model.onnx            (547 MB)
```

Para extrair:

```bash
unzip Em.Edith.2.zip
```
