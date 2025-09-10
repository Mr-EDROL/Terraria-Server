# Terraria-Server
Сервер для совместной удаленной игры

## Первичная подготовка
1. Создать необходимые папки (скоро будут в репозитории)
```bash
mkdir worlds config
```
2. Скипируйте карту в worlds
```bash
scp /path/to/world.wld user@host:/path/to/worlds/
```
3. Создам файл переменных окружения из шпблона
```bash
cp .env.dist .env
```
4. Указываем название мира и (опционально) прочие переменные (Полный список используемых переменных в ```docker-compose.yml```).
```bash
nano .env
```

## Запуск
```bash
docker compose up -d
```
