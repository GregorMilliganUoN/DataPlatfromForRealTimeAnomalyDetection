FROM python:3.7
RUN mkdir src
WORKDIR /src
COPY . /src
COPY requirements.txt .
RUN pip install -r requirements.txt
RUN pip install jupyter 
RUN pip install plotly==5.4.0
EXPOSE 8888


CMD [ "jupyter", "notebook", "--ip='*'", "--port=8888", "--no-browser", "--allow-root" ]

#docker run -p 8888:8888 -v /Users/gregormilligan/liveProject/jupyter:/src gregor/lp-jupyter


