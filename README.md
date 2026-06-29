# SUTDoko

## Setup

Follow these steps after cloning our repository if you want to run our code locally.
The latest weights are available in `experiments/runs/`.

### Web Application

Follow these steps if you want to run our web application locally.

1. Optionally, configure `experiments/config.toml`.
2. Optionally, run `app/build.py`.
3. Open `app/index.html`.

### Experiments

Follow these steps if you want to run our experiments locally.

1. Rename `experiments/.env.example` to `experiments/.env`.
2. Set `WANDB_API_KEY` in `experiments/.env` to working [Weights & Biases (W&B)](http://wandb.ai) API key.
3. Install packages in `experiments/requirements.txt`. For example:
```sh
cd experiments
pip install -r requirements.txt
```
4. Install [torch](https://pytorch.org/get-started/locally).
5. Run pipeline. For example:
```sh
python -B preprocess.py
python -B train.py
python -B test.py
```
