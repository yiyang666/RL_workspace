FROM rl_base:latest

# =========================
# RL Learning Dependencies
# =========================
COPY requirements.txt /tmp/requirements.txt

RUN pip install -r /tmp/requirements.txt

WORKDIR /workspace

CMD ["/bin/bash"]