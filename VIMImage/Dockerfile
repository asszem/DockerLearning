FROM alpine

COPY .bashrc-docker /root/.bashrc
COPY .vimrc-docker /root/.vimrc

RUN apk update && apk add --no-cache vim-tiny curl bash wget

#Set the shell to bash, set it as a loging shell, and source .bashrc from ~
#https://stackoverflow.com/questions/20635472/using-the-run-instruction-in-a-dockerfile-with-source-does-not-work/45087082#45087082

SHELL ["/bin/bash", "-l", "-c"]
CMD ["source .bashrc"]
CMD bash
