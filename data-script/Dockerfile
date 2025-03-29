FROM amazonlinux:2023
RUN dnf -y update && \
  dnf -y install mariadb105 && \
  dnf clean all
WORKDIR /opt
COPY mydatabase.sql import.sh /opt
RUN chmod +x import.sh
CMD ["sh", "import.sh"]