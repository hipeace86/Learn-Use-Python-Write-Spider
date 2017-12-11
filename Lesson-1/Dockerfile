FROM python:alpine3.6
MAINTAINER hipeace86 <hipeace86@gmail.com>
WORKDIR /data
ADD requirements.txt /root/
COPY jupyter_notebook_config.py /root/.jupyter/
RUN echo "http://mirrors.aliyun.com/alpine/v3.6/main/" > /etc/apk/repositories && \
    apk update && \
    apk add --no-cache cmake gcc libxml2-dev libxslt-dev g++ && \
    pip install --no-cache-dir -r /root/requirements.txt
# IPython NoteBook
EXPOSE 8888
# pyspider
EXPOSE 5000
# 示例程序中将会监听的端口
EXPOSE 8080
ENV PASSWORD "88888888"
CMD ["jupyter-notebook", "--no-browser","--allow-root"]