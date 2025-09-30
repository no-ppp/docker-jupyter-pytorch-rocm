# docker-jupyter-pytorch-rocm
Fast Docker setup for PyTorch with AMD GPU (ROCm) support in Jupyter Notebook.


# 🐳 docker-jupyter-pytorch-rocm

Fast Docker setup for running **PyTorch with AMD GPU (ROCm) support** inside **Jupyter Notebook**.

---

## ⚡ Features

* ✅ **ROCm-enabled PyTorch** for AMD GPU acceleration
* ✅ Preinstalled **Jupyter Notebook & JupyterLab**
* ✅ GPU access via `/dev/kfd` and `/dev/dri`
* ✅ Easy-to-use `docker-compose` workflow

---

## 🔧 Prerequisites

* [Docker](https://docs.docker.com/get-docker/) & [Docker Compose](https://docs.docker.com/compose/)
* AMD GPU with [ROCm](https://rocmdocs.amd.com/en/latest/) support
* Linux system (recommended for ROCm)

---

## 🚀 Setup Instructions

### 1️⃣ Build the Docker image

```bash
docker-compose build
```

---

### 2️⃣ Start Jupyter Notebook

```bash
docker-compose up
```

---

### 3️⃣ Access Jupyter Notebook

Open your browser and go to:

👉 [http://localhost:8888](http://localhost:8888)

Copy the **token** from the container logs if prompted. <-- By default it is set to "--NotebookApp.token=''" in dockerfile , change it if needed.

---

### 4️⃣ Stop the server

Press `Ctrl + C` in the terminal, then run:

```bash
docker-compose down
```

---

## 📝 Notes

* The container maps `/dev/kfd` and `/dev/dri` for AMD GPU access.
* Make sure your host system has **ROCm installed and supported hardware**.
* For troubleshooting, see:

  * [Docker documentation](https://docs.docker.com/)
  * [ROCm documentation](https://rocmdocs.amd.com/en/latest/)

---

## 📌 Tags

`#docker` `#jupyter` `#pytorch` `#rocm` `#amd-gpu` `#deep-learning` `#machine-learning`

