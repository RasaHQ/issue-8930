This repo was made to work on [this issue](https://github.com/RasaHQ/rasa/issues/8930). The issue is that that the `CRFEntityExtractor` seems to ignore featurizers while the docs say that they are used.

Here are some useful commands to run:

```
rasa test nlu --config config.yml --out gridresults/basic-config
rasa test nlu --config config-lm.yml --out gridresults/basic-config
time rasa test nlu --model models/config-base.tar.gz
time rasa test nlu --model models/config-lm.tar.gz
```