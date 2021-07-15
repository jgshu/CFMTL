# Clustered Federated Multi-Task Learning with Non-IID Data

## Environment

python 3.9.1

pytorch 1.7.1+cu101

## Run Experiments and Get Figures

### Performance

python main.py --dataset mnist --iid iid --ep 50 --local_ep 1 --frac 0.2 --num_batch 10 --num_clients 250 --clust 50 --L 1.0 --experiment performance-mnist --filename fig
python fig.py --experiment performance-mnist --filename fig

python main.py --dataset mnist --iid non-iid --ratio 0.25 --ep 50 --local_ep 1 --frac 0.2 --num_batch 10 --num_clients 250 --clust 50 --L 0.1 --experiment performance-mnist --filename fig
python fig.py --experiment performance-mnist --filename fig

python main.py --dataset mnist --iid non-iid --ratio 0.5 --ep 50 --local_ep 1 --frac 0.2 --num_batch 10 --num_clients 250 --clust 50 --L 0.1 --experiment performance-mnist --filename fig
python fig.py --experiment performance-mnist --filename fig

python main.py --dataset mnist --iid non-iid --ratio 0.75 --ep 50 --local_ep 1 --frac 0.2 --num_batch 10 --num_clients 250 --clust 50 --L 0.001 --experiment performance-mnist --filename fig
python fig.py --experiment performance-mnist --filename fig

python main.py --dataset mnist --iid non-iid-single_class --ep 50 --local_ep 1 --frac 0.2 --num_batch 10 --num_clients 250 --clust 50 --L 0.001 --experiment performance-mnist --filename fig
python fig.py --experiment performance-mnist --filename fig
