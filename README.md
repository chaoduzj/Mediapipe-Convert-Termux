# Mediapipe-Convert-Termux
I can't upload lots of models to huggingface it takes to much time. but it's easy to convert yourself. u probably need at least 8gb ram depending on how big the model is;)

Makesure you install UBUNTU FIRST:

pkg updated && pkg upgrade -y && termux-setup-storage && pkg install wget -y && pkg install git -y && pkg install proot -y && cd ~ && git clone https://github.com/MFDGaming/ubuntu-in-termux.git && cd ubuntu-in-termux && chmod +x ubuntu.sh && ./ubuntu.sh -y && ./startubuntu.sh

just put both covert.py files in the termux ubuntu root folder and create 2 folders inside the root folder name one ckpt and the other output,then make sure u put the safetensors you want to convert in the root folder then just copy the name of each model then paste one at a time for each conversion inside the ckpt-convert.py file ull see an model already inside just overwrite that model name don't overwrite the root name it should look like this: /root/DreamShaper_v_8.safetensors

save the ckpt-convert.py file then just run this command: python3 ckpt-convert.py && python3 convert.py --ckpt_path /root/ckpt/model.ckpt --output_path /root/output/


copy the whole command at once and paste it into termux then press enter.
