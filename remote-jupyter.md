# Working with a remote Jupyter notebook

In order to access an Ipython/Jupyter notebook running on a remote
server, follow these steps:

- ssh to the server while enabling port forwarding for a chosen port
  to your local machine. You can change the port number given below,
  it's just an example.

   ssh -L 5558:localhost:5558 yellow.uvt.nl

- On the remote server (yellow in this case) start up ipython (or
  jupyter), and specify the chosen port:

   ipython notebook --port 5558

- Open a browser and go to http://localhost:5558/
