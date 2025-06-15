# Brain tumor classification and evaluation using explainable deep learning techniques and segmentation

## Datasets
Multiple brain tumor datasets were used for this task, most of them are available only for classification tasks for supervised learning, but one (Figshare) also has segmentation information using masks which can be useful to evaluate how the classification models learned.

### Figshare: Brain tumor dataset
Consisting of a wide-ranging compilation of 3064 T1-weighted contrastenhanced MRI images captured in the form of two–dimensional (2D) slices with a resolution of 512×512 pixels, obtainined from sagittal, coronal, and axial planes and originated from a group of 233 patients diagnosed with three distinct types of BT: Glioma, Meningioma, and Pituitary tumor. 
Specifically, the dataset comprises 1426 slices corresponding to Glioma cases, 708 slices from patients with Meningioma, and 930 slices depicting Pituitary tumors.
All images were acquired after Gd-DTPA injection at Nanfang Hospital, Guangzhou, China and General Hospital, Tianjin Medical University, China from 2005.9 to 2010.10. The images have an in-plane resolution of 512 × 512 with pixel dimensions of 0.49 × 0.49 mm^2 . The slice thickness is 6 mm and the slice gap is 1 mm. The Gd dose was 0.1 mmol/kg at a rate of 2 ml/s. 

Available at: https://doi.org/10.6084/m9.figshare.1512427.v8

Cited by:

- S. A. Gore, A. S. Patil, A. S. Auti, A. D. Banne and H. S. Mali, "Brain Tumor Classification in MRI Scans Using Shape Features & Machine Learning Techniques," 2025 International Conference on Emerging Smart Computing and Informatics (ESCI), Pune, India, 2025, pp. 1-6, doi: 10.1109/ESCI63694.2025.10988081.
- N. Bansal, A. Khan, A. Tyagi, M. Goel, R. Baghel and S. Gupta, "Efficient and Accurate Brain Tumor Diagnosis: A CNN Approach for MRI Image Classification," 2025 3rd International Conference on Disruptive Technologies (ICDT), Greater Noida, India, 2025, pp. 1100-1102, doi: 10.1109/ICDT63985.2025.10986513.
- Y. Modaresnia, F. A. Torghabeh and S. A. Hosseini, "EfficientNetB0’s Hybrid Approach for Brain Tumor Classification from MRI Images Using Deep Learning and Bagging Trees," 2023 13th International Conference on Computer and Knowledge Engineering (ICCKE), Mashhad, Iran, Islamic Republic of, 2023, pp. 234-239, doi: 10.1109/ICCKE60553.2023.10326290.

### Kaggle: Brain Tumor MRI Dataset
Consists of 3 tumor datasets, contains 7023 images of human brain MRI images which are classified into 4 classes: glioma, meningioma, pituitary and no tumor.
No tumor class images were taken from the Br35H dataset. SARTAJ glioma class images were ignored due inconsistences found by the author.
Only classification information is available due limitations of the composed datasets.

Available at: https://doi.org/10.34740/kaggle/dsv/2645886

Composed by:
- Figshare: Brain tumor dataset 
- Kaggle: Brain Tumor Classification (MRI)
- Kaggle: Br35H :: Brain Tumor Detection 2020

#### Kaggle: Brain Tumor Classification (MRI)
Consisting of 2764 brain MRI slices with the same BT types as the first dataset. Being 926 Glioma, 937 Meningioma and 901 Pituitary cases, obtained from three axial planes.

Available at: https://doi.org/10.34740/kaggle/dsv/1183165

Cited by:
- Ravinder, M., Saluja, G., Allabun, S. et al. Enhanced brain tumor classification using graph convolutional neural network architecture. Sci Rep 13, 14938 (2023). https://doi.org/10.1038/s41598-023-41407-8
- Y. Modaresnia, F. A. Torghabeh and S. A. Hosseini, "EfficientNetB0’s Hybrid Approach for Brain Tumor Classification from MRI Images Using Deep Learning and Bagging Trees," 2023 13th International Conference on Computer and Knowledge Engineering (ICCKE), Mashhad, Iran, Islamic Republic of, 2023, pp. 234-239, doi: 10.1109/ICCKE60553.2023.10326290.

#### Kaggle: Br35H :: Brain Tumor Detection 2020
Contains 1500 MRI images classified as with tumor and 1500 MRI images without tumor.
There are no references about how the dataset was created and neither a DOI id for citation.

Available at: https://www.kaggle.com/datasets/ahmedhamada0/brain-tumor-detection

## Google Cloud Service
Given you are not running this code on a native environment on GCP you will need an application key and install the GCS connector on your cluster.
Use Maven: com.google.cloud.bigdataoss:gcs-connector:hadoop3-2.2.5
