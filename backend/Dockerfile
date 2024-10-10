# Sử dụng image node
FROM node:18

# Tạo thư mục làm việc cho ứng dụng
WORKDIR /usr/src/app

# Copy package.json và cài đặt các dependencies
COPY package*.json ./
RUN npm install

# Copy toàn bộ source code
COPY . .

# Build ứng dụng
RUN npm run build

# Lắng nghe trên cổng 3000
EXPOSE 3000

# Khởi chạy ứng dụng
CMD [ "npm", "run", "start:prod" ]
