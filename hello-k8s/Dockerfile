# 1. ใช้ Base Image ของ Node.js
FROM node:18-alpine

# 2. กำหนด Working Directory ภายใน Image
WORKDIR /app

# 3. Copy ไฟล์ package.json และติดตั้ง dependencies ก่อน
COPY package*.json ./
RUN npm install

# 4. Copy ไฟล์โค้ดทั้งหมดเข้ามา
COPY . .

# 5. บอกว่า Container จะทำงานที่ Port 3000
EXPOSE 3000

# 6. คำสั่งที่จะรันเมื่อ Container เริ่มทำงาน
CMD [ "npm", "start" ]