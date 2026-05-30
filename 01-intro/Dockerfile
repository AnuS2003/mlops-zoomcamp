FROM python:3.12-slim

WORKDIR /zoomcamp

# Add pandas, numpy, scikit-learn, and mlflow to the install list
RUN pip install --no-cache-dir \
    notebook \
    pandas \
    numpy \
    scikit-learn \
    mlflow \
    matplotlib

EXPOSE 8888
ENV PYTHONUNBUFFERED=1

CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--allow-root", "--no-browser", "--NotebookApp.token=", "--NotebookApp.password="]
