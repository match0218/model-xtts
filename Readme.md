# 1. Load Docker Image
`docker load -i ollama-tinyllama.tar`
# 2. run docker Image
`docker run --gpus all -it --entrypoint /bin/bash -v </path/to/.ollama>:/home ollama/ollama`
in docker console
`ollama serve`

# 3. connect docker container
`docker exec -it <container_id> /bin/bash` (get container id using `docker ps`)
in doker console
`cp /home/.ollama /root/.ollama -r`
`ollama run tinyllama`
