Are you wearing a mask? 

##############################################################
Fornita un immagine, l'applicazione identifica la presenza di un volto, e se questo indossa o meno una maschera.

##############################################################
Valorizzare la variabile "foo_img" presente nell'ultima cella del file "Script/facemask_infer.ipynb", con l'immagine da passare in input all'applicazione.

Nel caso si volesse acquisire un frame da webcam, attivare la cella "Acquisizione dell'immagine tramite webcam".

NOTA:
Assicurarsi che le variabili WGTS_PATH e face_cascade (quest'ultima presente in utilis.ipynb), puntino rispettivamente al file contenente i pesi (Dati/BestWeights/best_model.pt) e il file per la face-detection (Repo/FaceDetect-master/haarcascade_frontalface_default.xml)

##############################################################
Script: "Questa directory contiene gli script che compongono il progetto"
    - facemask_exp.ipynb: Esegue la K-Fold c.v. sul training-dataset.
    - facemask_train.ipynb: Esegue il training della rete sull'intero dataset.
    - facemask_test.ipynb: Esegue una ulteriore validazione del modello, utilizzando un test-dataset esterno.
    - facemask_infer.ipynb: Permette di fare inferenza su un immagine esterna, ripresa dalla webcam, o fornita in input valorizzando                                       l'apposita variabile "foo_img".
    - utils.ipynb: Insieme di funzioni richiamate negli script che compongono il progetto.
    - training_data_preparation.ipynb: Selezione e preparazione immagini per training-set.
    - test_data_preparation.ipynb: Selezione e preparazione immagini per test-set.
    - Results.csv: Riepilogo risultati degli esperimenti.
    
 Script/Imgs_infer: "Questa directory contiene un immagine campione, su cui fare inferenza"
    
 Dati: "Questa directory contiene le immagini del training e del test set. 
Inoltre, contiene i pesi salvati durante la fase di training della rete"
        
 Repo/FaceDetect-master: "Questa directory contiene il file 'haarcascade_frontalface_default.xml', necessario per effettuare la face-detection"