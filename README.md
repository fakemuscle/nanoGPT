git clone https://github.com/karpathy/nanoGPT
cd nanoGPT

pip install torch numpy matplotlib

git add .
git commit -m "Initial commit"
git remote add origin <your-repo-url>
git push -u origin main

python data/shakespeare_char/prepare.py
python train.py config/train_shakespeare_char.py
python sample.py --out_dir=out-shakespeare-char

