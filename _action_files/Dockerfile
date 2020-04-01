FROM hamelsmu/fastpages-nbdev

WORKDIR /fastpages
COPY . .
RUN chmod u+x action_entrypoint.sh
RUN chmod u+x word2post.sh
RUN pip install jupyter_contrib_nbextensions
RUN jupyter contrib nbextension install --user
RUN jupyter nbextension enable spellchecker/main

CMD [ "/fastpages/action_entrypoint.sh" ]
