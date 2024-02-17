# 1. load docker image
`docker load -i xtts-streaming-local.tar`

# 2. run docker image
`docker run --gpus=all -e COQUI_TOS_AGREED=1 --rm -p 8000:80 ghcr.io/coqui-ai/xtts-streaming-local:latest`
