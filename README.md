# e-Breath Dataset
The **e-Breath Dataset** contains breath sound and non-breath sound. The data of breath sound is collected from 14 persons worn the mobile devices several hours and perform daily activities such as sitting, walking, running, cleaning and playing sports. The breath sounds from the subject were recorded from 10 to 15 minutes for each activity. The non-breath sound are any events out of the breath including silent and ambient noises.
#### Datatype
Audio of this dataset is recorded with **16000Hz** sample rate, and **wav** format
#### Database structure
```sh
eBreath-dataset/
├── annotated_breath
│   ├── ......
│   ├── uttxxx.wav
│   └── uttxxx.txt
└── segmented_4s
    ├── breath
    │   ├── ......
    │   ├── breath1.wav
    │   └── breath2.wav
    └── non-breath
        ├── ......
        ├── non-breath1.wav
        └── non-breath2.wav
```
The folder **annotated_breath** containing list of raw recording breath audio and its annotated label. Each wav audio file in this folder is corresponding to one utterance.
\
The folder **segmented_4s** containing a list of **4-second** segmentation of audio, divided into 2 label: breath, and non-breath. Each file have wav format, with 16000Hz sample rate