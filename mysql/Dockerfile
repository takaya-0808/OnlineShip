FROM mysql/mysql-server:8.0

EXPOSE 3306

ENV MYSQL_DATABASE=OnlineShop \
  MYSQL_USER=root \
  MYSQL_PASSWORD=root \
  MYSQL_ROOT_PASSWORD=root \
  TZ=Asia/Tokyo

COPY ./my.cnf /etc/mysql/my.cnf

RUN chmod 644 /etc/mysql/my.cnf

COPY ./sql /docker-entrypoint-initdb.d