# squeezenet

This repository hosts the contributor source files for the squeezenet model. ModelHub integrates these files into an engine and controlled runtime environment. A unified API allows for out-of-the-box reproducible implementations of published models. For more information, please visit [www.modelhub.ai](http://modelhub.ai/) or contact us [info@modelhub.ai](mailto:info@modelhub.ai).

## meta

|                  |                                      |
| ---------------- | ------------------------------------ |
| id               | d50796da-87f2-4493-846e-6eeb498acc63 |
| application_area | ImageNet                             |
| task             | Classification                       |
| task_extended    | ImageNet classification              |
| data_type        | Image/Photo                          |
| data_source      | http://www.image-net.org/            |

## publication

|                |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| title          | SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| source         | arXiv                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| url | https://arxiv.org/abs/1602.07360 |
| year           | 2016                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| authors        | Forrest N. Iandola, Song Han, Matthew W. Moskewicz, Khalid Ashraf, William J. Dally, Kurt Keutzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| abstract       | Recent research on deep neural networks has focused primarily on improving accuracy. For a given accuracy level, it is typically possible to identify multiple DNN architectures that achieve that accuracy level. With equivalent accuracy, smaller DNN architectures offer at least three advantages: (1) Smaller DNNs require less communication across servers during distributed training. (2) Smaller DNNs require less bandwidth to export a new model from the cloud to an autonomous car. (3) Smaller DNNs are more feasible to deploy on FPGAs and other hardware with limited memory. To provide all of these advantages, we propose a small DNN architecture called SqueezeNet. SqueezeNet achieves AlexNet-level accuracy on ImageNet with 50x fewer parameters. Additionally, with model compression techniques we are able to compress SqueezeNet to less than 0.5MB (510x smaller than AlexNet). |
| google_scholar | https://scholar.google.com/scholar?cites=17131899958223648583&as_sdt=40000005&sciodt=0,22&hl=en                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| bibtex         | @article{iandola2016squeezenet, title={SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and< 0.5 MB model size}, author={Iandola, Forrest N and Han, Song and Moskewicz, Matthew W and Ashraf, Khalid and Dally, William J and Keutzer, Kurt}, journal={arXiv preprint arXiv:1602.07360}, year={2016}}                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

## model

|               |                                                                                                                                                                                                                                                                                                                                                         |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| description   | SqueezeNet begins with a standalone convolution layer (conv1), followed by 8 Fire modules (fire2-9), ending with a final conv layer (conv10). We gradually increase the number of filters per fire module from the beginning to the end of the network. SqueezeNet performs max-pooling with a stride of 2 after layers conv1, fire4, fire8, and conv10 |
| architecture  | Convolutional Neural Network (CNN)                                                                                                                                                                                                                                                                                                                      |
| learning_type | Supervised learning                                                                                                                                                                                                                                                                                                                                     |
| format        | .onnx                                                                                                                                                                                                                                                                                                                                                   |
| I/O           | model I/O can be viewed [here](contrib_src/model/config.json)                                                                                                                                                                                                                                                                                           |
| license       | model license can be viewed [here](contrib_src/license/model)                                                                                                                                                                                                                                                                                           |

## run

To run this model and view others in the collection, view the instructions on [ModelHub](http://app.modelhub.ai/).

## contribute

To contribute models, visit the [ModelHub docs](https://modelhub.readthedocs.io/en/latest/).
