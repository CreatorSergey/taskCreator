# taskCreator
система управления задачами



### Сборка

1. установите обязательно пакет postgresql-server-dev-12

https://www.postgresql.org/download/linux/debian/

2. скачать git clone https://github.com/jtv/libpqxx.git

3. инструкция по сборке https://github.com/jtv/libpqxx/blob/master/BUILDING-cmake.md



4. зайти в папку

`cmake .`

`sudo cmake --build .`

`sudo cmake --install .`



### Запуск базы

By default, the postgres user has no password and can hence only connect if ran by the postgres system user. The following command will assign it:

```
sudo -u postgres psql -c "ALTER USER postgres PASSWORD 'postgres';"
sudo -u postgres psql -c "CREATE DATABASE testdb;"
```

- Start the PostgreSQL server

```
sudo service postgresql start
```

- Stop the PostgreSQL server:

```
sudo service postgresql stop
```
