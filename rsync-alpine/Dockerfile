FROM alpine:latest

# Install packages
RUN apk --no-cache add busybox-initscripts rsync

# Copy script which should be run
# Run the cron every minute
# COPY rsync-cron /etc/crontabs/root
COPY rsync-cron /etc/crontabs/root

CMD ["crond", "-l", "2", "-f"]