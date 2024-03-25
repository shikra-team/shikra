# Git LFS on Mac
brew install git-lfs
git lfs install
git lfs install --system

# Download LLAMA 7B Huggingface
git clone https://huggingface.co/huggyllama/llama-7b

# Download the Shikra Weights
python mllm/models/shikra/apply_delta.py \
    --base /path/to/llama-7b \
    --target /output/path/to/shikra-7b \
    --delta shikras/shikra-7b-delta-v1-0708