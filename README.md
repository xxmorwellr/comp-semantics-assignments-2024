## Environment configuration
- Using GPUs will make things run faster.

We can access the server by using SSH: `ssh -L 8888:localhost:8888 [your_x_account]@mltgpu.flov.gu.se -p 62266`

`ssh` tells the computer to connect remotely to the server.

`-L 8888:localhost:8888` allows us to connect using jupyter notebooks, remove it if you don't want to do that.

`-p 62266` tells the server to give your access through port 62266.

- Pay attention to PyTorch-GPU compatibility!

To set up a virtual environment on the server is suggested:

`pip install virtualenv`

`python -m venv nlp # Create a virtual environment folder nlp under the current path`

`conda activate nlp # activate the virtual environment`

`pip install numpy jupyter # install necessary packages in your own virtual env`

`pip install torch torchvision torchaudio # install pytorch & cuda (make sure compatibility, avoid calling from external env)`

`conda deactivate # exit virtual env`

- Check memory and current jobs in jupyter notebook:

`!nvidia-smi`

`!ps -aux | grep python`




