# Используем официальный образ Node.js
FROM node:14

# Создаем рабочую директорию
WORKDIR /usr/src/app

# Копируем package.json и package-lock.json
COPY package*.json ./

# Устанавливаем зависимости
RUN npm install

# Копируем исходный код
COPY . .

# Указываем команду для запуска приложения
CMD ["node", "src/app.js"]

# Открываем порт
EXPOSE 3000
