## Build

```
docker build -t react-app .
```

## Run

`-it` - интерактивный режим
`--rm` - удаляем контейнер после стопа
`-p` - 3000 порт занят, меняем на 3001

остальное в приложенной ссылке

```
sudo docker run -it --rm -v ${PWD}:/app -v /app/node_modules -p 3001:3000 -e CHOKIDAR_USEPOLLING=true react-app
```

Ссылка для чтения:

https://mherman.org/blog/dockerizing-a-react-app/