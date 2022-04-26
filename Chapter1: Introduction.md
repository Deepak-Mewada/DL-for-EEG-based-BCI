# DL-for-EEG-based-BCI

### Chapter1: Introduction

### Chapter1 
#### Background on BCI
BCi System translate human brain patterns into message or commands for trans,mission to the outer world(lotte,2018).
Generalized form of BCI: BCI system enables bidirectrional communication between the human brain and the computer.

Brain signals->collection->preprocessing->feature engineering->classification->control command->smart eruipmrnt->feedback

EEG signal: meausres the voltage fluctutation rsulting from ionic current within the neurons of the brain , require placing a series of electrodes on to the scalp to record the electrical brqain activity.
-ionic current generated within the brain is measured at the scalp, intervening matter(skull) greatly decrease the signal quality.-Needs preprocesssing to increase SNR

PREPROCESSING: 1.Signal cleaning: Smoothening the noisy signals or resolving the inconsistencies
               2. signal Normalization: normalizing each channel of the signals along the time axis
               3. Signal Enhancement : Removing direct curent
               4. Signal Reduction: Presenting a reduced representation of the sinal

Feature Engineering: FE refers to the process of extracting discriminating features from the inpout signals using domain knowledge.
              Traditional features:
                1.Time Domain: Variance,mean value,kurtosis     
                2.Frquency Domain ; fast fourior transform
                1.Time & Frequency Domain: discrete wavelet transform
              Drawback: -FE is highly dependent on domain knowledge
                        -Time Consuming
                        -May be inaccurate                        
 Hence the need for automatic extraction of distinguishable feature?               

##### 1.2: Why Deep learning?
Challanges of BCI Sys:
    1.Currupted: brain signals are easily currepted by various bilogical(e.g. eye blick,muscles artifects,fatigue and concentration level) and environmental artifects(e.g noise).
       As a result of thois brain signals face the challange of low SNR -->Need to learn informative representation from currupte brain signals.
    2.Human expertise to exteract features: time contraint due to expert less availability
        So need of a novel method that can automatically extract the most representative features from the input data is highly desirable.
    3.Dealing with dynamic data stream: most ML research yet focused on static data therefor they,cannot accurately classify rapidly changing brain signals.
        -Need of novel learning methods
    4. labeling of data is required:improving the performance of BCI system by including information contained within the unlabled data is crucial.


    DEEP LEARNING:
    DL learns informative representation from the input data by building hierarchical networks.
    DL can learn high level and complicated representation by combining a number of simpler representations while each simpler representation extracts partial information relating to the complex information.

    Advantage of DL:
    1. Works directly on raw signals.
    2. Back propagation: allows to learn high auality representation even though the input is corrupted or noisy.
    3. DNN can capture both representative high level features and latent dependencoies through deep steuctures.

Why this Book?

