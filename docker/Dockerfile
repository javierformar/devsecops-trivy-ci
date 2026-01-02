FROM alpine:3.23.2

RUN addgroup -S appgroup && adduser -S appuser -G appgroup

RUN apk add --no-cache curl

WORKDIR /app 

COPY --chmod=755 app/app.sh /app/app.sh

USER appuser

CMD ["/app/app.sh"]
