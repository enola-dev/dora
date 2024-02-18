# Usage

## Generate YAML from MD

```bash
$ enola rosetta --in=github.md --out=BUILT?mediaType=application/yaml&proto-message=dev.enola.markdown.Markdowns
```

produces ~~(BTW note the `proto-message` header)~~:

```yaml !import OUT/github.yaml
```

## Generate YAMLs from MDs

```bash
$ enola rosetta --in=*.md --out=BUILT?mediaType=application/yaml&proto-message=dev.enola.markdown.Markdowns
```

## Generate RDF from YAML (ex-MD)

```bash
$ enola rosetta --in=BUILT/*.yaml --out=BUILT?mediaType=text/turtle
```

## Generate Graph

```bash
$ enola rosetta --in=BUILT/*.turtle --out=graph.gexf
```
