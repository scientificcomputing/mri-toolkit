---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Datasets

The `datasets` subcommand provides tools for listing and downloading example datasets.


```{code-cell} shell
!mritk datasets --help
```

To list available datasets, use:

```bash
mritk datasets list
```
You can also get more information about a specific dataset:

```bash
mritk datasets info <dataset_name>
```

To download a dataset, use:

```bash
mritk datasets download <dataset_name> -o /path/to/download
```

![data](https://github.com/user-attachments/assets/7e35f2d8-ca97-42e7-b9b9-3b609ba5148f)

It is also possible to only download a subset of a dataset using the `--subset` flag. For example if you only want to download the `surfaces` and `mesh-data` from the `gonzo` dataset you can do
```bash
mritk datasets download gonzo -o gonzo-data --subset surfaces.zip --subset mesh-data.zip
```
