# meg_application

A bash application for automating machine learning analysis for MEG connection data

------ Version History ------

- 0.0.3 (July.10.2019)
  - General updates
    - The non-2D applications now able to take node file
      - All related sh and R files updated for this update
    - SVM process now export the nested cross-validation results as part of the model files
    - Directory structure updated
    - R files put to the folder: R_files
      - All sh files updated for this change

  - New module connectivity_ml_2d.sh added
    - input_dat_process_2d.R added

  - New module connectivity_ml_reg_2d.sh added
    - reg_input_dat_process_2d.R added

  - Updates to connectivity_ml.sh (and the associated R modules)
    - Updates to connectivity_ml.sh
      - Check added for annotation file and input sample size

    - Updates to input_dat_process.R
      - Check added for annotation file and input sample size

  - Updates to connectivity_ml_reg.sh (and the associated R modules)
    - Updates to connectivity_ml_reg.sh
      - Check added for annotation file and input sample size

    - Updates to reg_input_dat_process.R
      - Check added for annotation file and input sample size

  - A bugs fixed for reg_ml_svm.R, now with correct error metric

- 0.0.2 (May.22.2019)
  - Updates to connectivity_ml.sh (and the associated R modules)
    - Updates to univariate.R
      - Weights now incorporated for univariate analysis

  - Updates to connectivity_ml_reg.sh (and the associated R modules)
    - Updates to reg_univariate.R
      - Weights now incorporated for univariate analysis

    - Updates to reg_ml_svm.R
      - Hierarchical clustering added after SVM
      - Subsetted data with selected connections now exported as a CSV file for the subsequent deep learning steps
      - Code base optimization

  - Version bumped to 0.0.2 for all modules

  - Bug fixes

- 0.0.1
  - Initial commit
