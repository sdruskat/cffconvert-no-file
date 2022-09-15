# cffconvert-no-file

A demo repository showing how to use the [cffconvert GitHub Action](https://github.com/marketplace/actions/cffconvert) to fail builds when no `CITATION.cff` file in the [Citation File Format](https://citation-file-format.github.io/) is present in a repository.

If you set up the action, so that it doesn't check only on pushes of the `./CITATION.cff` path (see [configuration in this repository](https://github.com/sdruskat/cffconvert-no-file/blob/fbe2ba46e9b940b9e031efb1d05866876ffb36dd/.github/workflows/cffconvert.yml#L1-L4)), the action will detect the absence of a `CITATION.cff` file and fail:

```yaml
name: cffconvert

on:
  push
```
