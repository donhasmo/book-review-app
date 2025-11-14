# Use Node.js LTS as base image
FROM node:18

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# Build Next.js production bundle
RUN npm run build

EXPOSE 3000

# Start Next.js production server
CMD ["npm", "start"]
