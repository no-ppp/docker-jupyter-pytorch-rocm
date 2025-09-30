FROM rocm/pytorch:latest

WORKDIR /workspace
RUN pip3 install jupyter notebook ipykernel
RUN python3 -m ipykernel install --user

EXPOSE 8888

CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root", "--NotebookApp.token=''"]
