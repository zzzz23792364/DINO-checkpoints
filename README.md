# DINO Checkpoints

Unofficial mirror of pretrained checkpoints from
[IDEA-Research/DINO](https://github.com/IDEA-Research/DINO), hosted as GitHub
Release assets. The weight file is ~536 MB, which exceeds GitHub's 100 MB limit
for files committed to a git repository, so it is distributed as a release
asset (2 GB per-file limit) instead of being tracked in git.

## Available checkpoints

| File | Model | Backbone | Epochs | Scales | COCO val AP | Size |
| --- | --- | --- | --- | --- | --- | --- |
| [`checkpoint0011_4scale.pth`](https://github.com/zzzz23792364/DINO-checkpoints/releases/download/v1.0/checkpoint0011_4scale.pth) | DINO | ResNet-50 | 12 | 4 | 49.0 | 535.7 MB (561,773,961 bytes) |

SHA256:

```text
0bcd6b0c33d60ed33461ce6f02ce5797a819c7c02eb7e15b76adfb6df307955a  checkpoint0011_4scale.pth
```

## Download

```sh
curl -L -O https://github.com/zzzz23792364/DINO-checkpoints/releases/download/v1.0/checkpoint0011_4scale.pth
```

Verify the download:

```sh
sha256sum -c checkpoint0011_4scale.pth.sha256
```

## Usage

The checkpoint follows the official DINO evaluation procedure:

```sh
git clone https://github.com/IDEA-Research/DINO.git
cd DINO
bash scripts/DINO_eval.sh /path/to/COCODIR /path/to/checkpoint0011_4scale.pth
```

Expected result: final AP about 49.0 on COCO val2017.

## Provenance

- Original source: official DINO model zoo
  ([Google Drive folder](https://drive.google.com/drive/folders/1qD5m1NmK0kjE5hh-G17XUX751WsEG-h_?usp=sharing)),
  file `checkpoint0011_4scale.pth` (last modified 2022-07-09).
- The file is mirrored unmodified. SHA256 above was computed after download.
- DINO is released under the [Apache License 2.0](https://github.com/IDEA-Research/DINO/blob/main/LICENSE).
  All credit belongs to the DINO authors (IDEA-Research). This repository only
  provides a mirror for convenience.
