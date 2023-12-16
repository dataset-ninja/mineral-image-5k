Dataset **MineralImage5k** can be downloaded in [Supervisely format](https://developer.supervisely.com/api-references/supervisely-annotation-json-format):

 [Download](https://assets.supervisely.com/supervisely-supervisely-assets-public/teams_storage/R/R/RG/Nx3Z71UDLE1Xnc9MFub0nvxFvQfLWI8OkGPPh0uRF13CWEeKDTtx4J3WsuLqMC60gNCOzXohHQBVpZaIolPGfKK0UGLNohg1T97rqqKRJN5Rw4QimY117kwwm1NR.tar)

As an alternative, it can be downloaded with *dataset-tools* package:
``` bash
pip install --upgrade dataset-tools
```

... using following python code:
``` python
import dataset_tools as dtools

dtools.download(dataset='MineralImage5k', dst_dir='~/dataset-ninja/')
```
Make sure not to overlook the [python code example](https://developer.supervisely.com/getting-started/python-sdk-tutorials/iterate-over-a-local-project) available on the Supervisely Developer Portal. It will give you a clear idea of how to effortlessly work with the downloaded dataset.

The data in original format can be [downloaded here](https://disk.yandex.ru/d/KapicF_MEysifg).