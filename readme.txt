Skin Cancer Capstone_Sept24.pdf - project report
Udacity ML Engineer  Capstone Proposal.pdf - approval proposal
Reviewer's comments: https://review.udacity.com/?utm_campaign=ret_000_auto_ndxxx_submission-reviewed&utm_source=blueshift&utm_medium=email&utm_content=reviewsapp-submission-reviewed&bsft_clkid=8ccbc573-8c83-4894-ba62-8022923ce038&bsft_uid=fec8a6f6-33c1-49f5-8436-c6d7238375d4&bsft_mid=7d439f83-791d-4953-9477-b27e47562ce2&bsft_eid=6f154690-7543-4582-9be7-e397af208dbd&bsft_txnid=3fc8293b-ea71-42aa-a102-9d88384b2227#!/reviews/1422085



cifar - directory for cifar-10 images in PNG format
Test_Data_Sq_orig - original 2017 ISIC 600 test data that have been cropped and resized to 300x300 pixels
Validation_Data_Sq_orig - original 2017 ISIC 150 validation data that have been cropped and resized to 300x300 pixels
Training_Data_Sq_orig_added_images - 5,000 images altogether from oversampling original 2,000 images, rotated
CLR - contain the cyclic learning rate code with proper licensing term and condition

ISIC_features-All-in-One.ipynb - features extraction
top_model_base-ISIC-AUC-All-in-One-plots-CV.ipynb  - conduct 5-folds CV analyes
top_model_base-ISIC-AUC-All-in-One-stacking-different_models.ipynb  - train a stacked ensemble

fine_tune-CLR-benchmark-with-VGG_and_ResNet50-CIFAR10.ipynb - fine tuning for the CIFAR-10 dataset
fine_tune-CLR-ISIC-with-VGG_Layer_1.ipynb  - VGG16 fine tuning for the 2017 ISIC cancer dataset


To extract features and train top models, please follow the steps:
(1) set parameters in "ISIC_features-All-in-One.ipynb" then run the program
(2) it should generate multiple output files, depending on how many models are chosen
(3) run either "top_model_base-ISIC-AUC-All-in-One-plots-CV.ipynb" or "top_model_base-ISIC-AUC-All-in-One-stacking-different_models.ipynb"

For fine tuning:
(1) set parameters in the notebook
(2) run the notework, it will read image files directly from different directories


