FROM postgres:15

ARG USER
ARG USER_ID

RUN useradd -m -u ${USER_ID} -G root $USER

USER $USER

ENTRYPOINT ["docker-entrypoint.sh"]

CMD ["postgres"]
