FROM alpine
COPY ./ragamicro /app/ragamicro
RUN chmod +x /app/ragamicro
RUN apk add --no-cache libc6-compat
ENV PORT 8080
EXPOSE 8080
ENTRYPOINT /app/ragamicro