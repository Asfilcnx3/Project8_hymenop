# Project8_hymenoptera

## Español
> En este proyecto utilicé solo una red neuronal simple con 2 salidas para una clasificación binaria pero con un entrenamiento con "transfer learning" del modelo "IMAGENET1K_V2" que fue preentrenado para clasificación de imagenes. 

## English
> In this project i only use a simple RNN with 2 outputs to do a binary classification but using "Transfer Learning" of the model "IMAGENET1K_V2" that was pretrained to image classification.

## Descripción / Description
> - Este es un proyecto de visión por computadora con torch.cuda para acelerar manualmente el entrenamiento. Este proyecto es para hacer la comparación entre "congelar" las capas de atención y seguirlas entrenando. 
> 
> - Se utilizó PyTorch como herramienta principal y el set de datos "hymenoptera" que encontrarás en este mismo repositorio.
> 
> - Se Trabajó con muy poca Data Augmentation. Solo 2 capas y la normalización.
> 
> - Se usó EarlyStopping a 7 épocas de paciencia.
> 
> - 30 épocas de entrenamiento totales para ambos modelos.
> 
> - BatchSize de 4 imagenes.
> 
> - Únicamente trabajamos la validación y entrenamiento en este proyecto.

> -------------------

> - This is a computer vision project using torch.cude to manually accelerate the training loop. This project is to compare the accuracy between "Fine Tuning" and "Feature Extraction".
> 
> - Using PyTorch as main tool and the "hymenoptera" dataset that you can find in this repo.
> 
> - Worked with only 2 layers of Data Augmentation and the normalize layer.
> 
> - EarlyStopping was used with 7 patience epochs.
> 
> - 30 total epochs for both models.
>
> - BatchSize = 4
>
> - Only worked with train and validation data.

## Tecnologías usadas / Used Technologies
- Python (main)
- PyTorch
- Google Colab / Jupyter NoteBook
- Matplotlib, Seaborn
- Sklearn
- CUDA

## Final Results / Resultados Finales
Classification report Fine Tuning:
           
                   precision    recall  f1-score   support

            ants       0.99      0.97      0.98        70
            bees       0.98      0.99      0.98        83

        accuracy                           0.98       153
       macro avg       0.98      0.98      0.98       153
    weighted avg       0.98      0.98      0.98       153

Classification report Feature Extraction:

                   precision    recall  f1-score   support

            ants       0.99      0.96      0.97        70
            bees       0.96      0.99      0.98        83

        accuracy                           0.97       153
       macro avg       0.98      0.97      0.97       153
    weighted avg       0.97      0.97      0.97       153
