Dataset **MineralImage5k** can be downloaded in [Supervisely format](https://developer.supervisely.com/api-references/supervisely-annotation-json-format):

 [Download](https://assets.supervisely.com/remote/eyJsaW5rIjogInMzOi8vc3VwZXJ2aXNlbHktZGF0YXNldHMvMzE1Nl9NaW5lcmFsSW1hZ2U1ay9taW5lcmFsaW1hZ2U1ay1EYXRhc2V0TmluamEudGFyIiwgInNpZyI6ICJnSTAwSWlBQUU5QzRVWjliU2RZNWhvRmhzbnQ5aDZIT04xMWNxR1RXVHdBPSJ9?response-content-disposition=attachment%3B%20filename%3D%22mineralimage5k-DatasetNinja.tar%22)

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