FROM quay.io/mbayser/jupyter-max:1

# install - requirements.txt
COPY --chown=jovyan:users requirements.txt /tmp/requirements.txt
RUN python3 -m pip install -r /tmp/requirements.txt --quiet --no-cache-dir \
 && rm -f /tmp/requirements.txt

COPY --chown=jovyan:users s6/ /etc
