# textlint
# docker run --rm -it pottava/textlint:10.2
# docker run --rm -it -v $(pwd):/work pottava/textlint:10.2 .

FROM node:9.11-alpine

ENV TEXTLINT_VERSION=10.2.1

RUN yarn global add "textlint@${TEXTLINT_VERSION}" \
    && rm -rf /usr/local/share/.cache

ENTRYPOINT ["textlint"]
CMD ["."]
