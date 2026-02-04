# Experiment on Molecular Dynamics Simulation

## Code based on [Equiformer Implementation](https://github.com/atomicarchitects/equiformer)

For an example training on MD17, with aspirin as the target molecule run:

```
python main_md17.py     --output-dir 'models/md17/equiformer/se_l2/target@aspirin/reg_aspirin_1500_epochs'     --model-name 'graph_attention_transformer_nonlinear_exp_l2_md17'     --input-irreps '64x0e'     --target 'aspirin'     --data-path 'datasets/md17'     --epochs 1500     --lr 5e-4     --batch-size 8     --weight-decay 1e-6     --num-basis 32     --energy-weight 1     --force-weight 80  --test-interval 20

```

similar for other molecules follow the scripts in [scripts/train/md17/equiformer/se_l2](https://github.com/StefanosPert/Equivariant_Optimization_CR/tree/main/MoleculeDyn/scripts/train/md17/equiformer/se_l2)
