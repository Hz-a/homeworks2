
# HOOD: Hierarchical Graphs for Generalized Modelling of Clothing Dynamics


$HOOD_DATA
    |-- aux_data
        |-- datasplits // directory with csv data splits used for training the model
        |-- smpl // directory with smpl models
            |-- SMPL_NEUTRAL.pkl
            |-- SMPL_FEMALE.pkl
            |-- SMPL_MALE.pkl
        |-- garment_meshes // folder with .obj meshes for garments used in HOOD
        |-- garments_dict.pkl // dictionary with garmentmeshes and their auxilliary data used for training and inference
        |-- smpl_aux.pkl // dictionary with indices of SMPL vertices that correspond to hands, used to disable hands during inference to avoid body self-intersections
    |-- trained_models // directory with trained HOOD models
        |-- cvpr_submission.pth // model used in the CVPR paper
        |-- postcvpr.pth // model trained with refactored code with several bug fixes after the CVPR submission
        |-- fine15.pth // baseline model without denoted as "Fine15" in the paper (15 message-passing steps, no long-range edges)
        |-- fine48.pth // baseline model without denoted as "Fine48" in the paper (48 message-passing steps, no long-range edges)
```

