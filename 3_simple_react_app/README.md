## Build

```
docker build -t react-app .
```

## Run

`-it` - интерактивный режим
`--rm` - удаляем контейнер после стопа
`-p` - 3000 порт занят, меняем на 3001

```
docker run -it --rm -p 3001:3000 react-app
```

Ссылка для чтения:

https://mherman.org/blog/dockerizing-a-react-app/