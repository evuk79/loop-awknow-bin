# loop-awknow-bin

Artifact temporal de publicación para `loop-awknow` (agente ACP de
`awknow-rs`), usado
por la integración Harbor / Terminal-Bench del doc 574.

**No es el código fuente.** El código vive en el repositorio principal de
makoraga. Acá solo vive el binario compilado, como release asset, porque el
instalador del agente ACP nativo de Harbor exige una URL HTTPS pública
(`AcpBinaryTarget.archive`) y descarga sin token.

## Uso

```
https://github.com/evuk79/loop-awknow-bin/releases/download/f574/loop-awknow.tar.gz
```

## Verificación

El checksum que Harbor valida es **el del archivo `.tar.gz`**, no el del binario
suelto:

```
sha256  3ae4756e1004b3a2b0f0e982c6b4e6ffacbea03cb8bbc0f47de2f46f28aa9033  loop-awknow.tar.gz
```

## Vida útil

Repo **efímero**: se borra al terminar la medición del piloto. Si el release ya
no se necesita, se puede eliminar este repositorio entero.