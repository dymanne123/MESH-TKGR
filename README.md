Code implementation for MESH

Run the experiments by: 
```
cd ./src
python main_llm_mmoe_norm.py -d ICEWS14s --train-history-len 3 --test-history-len 3 --dilate-len 1 --lr 0.001 --n-layers 2 --evaluate-every 1 --gpu=0 --n-hidden 100 --self-loop --decoder convtranse --encoder uvrgcn --layer-norm --weight 0.5  --entity-prediction --relation-prediction --add-static-graph --angle 10 --discount 1 --task-weight 0.7 --weight_loss 1
```

Due to GitHub's file size limitations, you can find the graph encoder and LLM embedding files (LLaMA2-7B) we used at this link and place them in the models folder: https://drive.google.com/drive/folders/1secSnfOxbLeYfzZdd14NnMbGpZ8iJ3Gj?usp=drive_link
You can also use other graph encoder or embeddings from different LLMs.
