# Public product assets

Public documentation and media used outside their source repositories. Product source can remain private.

## Catalog

| Family | Product | Inventory and usage |
| --- | --- | --- |
| VS Code | Local Change Guard | [Product directory](vscode/local-change-guard/README.md) |

## Folder convention

`<family>/<product>/releases/<version>/`

- **Family** is the distribution channel or product family, such as `vscode`.
- **Product** is a stable lowercase product slug, such as `local-change-guard`.
- **Version** matches the product version documented by that snapshot.
- A product-level `README.md` lists its versions, consumers and legacy URLs.
- Each version has a `manifest.json`: source repository/path, public file path, usage and SHA-256 for every mirrored file.

## Adding or updating a share

1. Add the product to this catalog and create its product index.
2. Copy only reviewed public documentation/media; keep relative paths from source where possible.
3. Record every file's source, usage and hash in the version manifest. Include licensing and attribution needed by that share.
4. Check links and images without authentication before distributing a consumer package.
5. Keep old URLs working. Once a product version is released, publish later changes under a new version instead of replacing that snapshot.

Source repositories own the content. This repository distributes reviewed copies; it is not a second authoring source. Never copy credentials, personal work records, local paths, customer data or private implementation files here.
