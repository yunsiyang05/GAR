# GAR
This is the official code of GAR.

## Usage
1. Go to the `PGE` package and use 
`python3 plainagg.py --dataset CiteULike --emb node2vec` 
to construct *PGE* for your dataset.

2. Go to the `GCGAN` package and run *GAR-GNN* and *GAR-MLP*
   - GAR-GNN:
   
      ```python3 main.py --gpu_id 0 --dataset CiteULike --embed_meth node2vec --gan_model gargnn --sim_coe 0.05 --alpha 0.9```

   - GAR-MLP:
   
      ```python3 main.py --gpu_id 0 --dataset CiteULike --embed_meth node2vec --agg_meth none --gan_model garmlp --real_lys [200,200] --real_act tanh --sim_coe 0.1```

   
