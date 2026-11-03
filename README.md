# avalorium-assets

Assets baixados sob demanda pelo cliente AvaloriumOTC. Os arquivos ficam nos **Releases**, não no histórico do git.

## Minimapa HD (`hdmap-1525-vN`)

- `hdmap-1525-vN.zip`: pack do minimapa HD (cifrado, sem compressão), extraído pelo cliente em `<pasta de escrita>/things/1525/satellite/`.
- `hdmap-manifest.json`: `version`, `url`, `size`, `sha256`, `files`, `installSize`.

O cliente lê sempre `releases/latest/download/hdmap-manifest.json`. Para publicar uma versão nova, gere o pack no repositório do cliente com `python tools/minimap_hd/package_pack.py --version N` e crie um release novo com os dois arquivos.
