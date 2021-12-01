FROM python:3.9
RUN mkdir src
WORKDIR /src
COPY . /src
RUN pip install --upgrade pip 
RUN pip --no-cache-dir install jupyter
EXPOSE 8888
CMD [ "jupyter", "notebook", "--ip='*'", "--port=8888", "--no-browser", "--allow-root" ]
