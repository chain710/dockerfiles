FROM ghcr.io/chain710/comfyui-torch:py3.12.4-cu121
ARG CHECKOUT=master
WORKDIR /app
RUN git clone https://github.com/comfyanonymous/ComfyUI.git . &&  git checkout ${CHECKOUT} && pip install -r requirements.txt --no-cache-dir
ENTRYPOINT [ "python", "/app/main.py" ]