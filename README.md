tải về thay thế, sau đó chạy lại lệnh 
python3 -m venv .venv && . .venv/bin/activate && ./run_rl_swarm.sh
gỡ bỏ torch và thay thế torch cpu nếu vẫn nhận gpu
pip uninstall torchvision
pip install torch==2.6.0+cpu --index-url https://download.pytorch.org/whl/cpu
python -c "import torch; print(torch.__version__); print(torch.cuda.is_available())"
nếu xuất hiện lỗi vllm thì gỡ luôn
pip uninstall vllm
