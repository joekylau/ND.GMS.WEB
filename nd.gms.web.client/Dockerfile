FROM node:13.10.1

# Set working directory to /app
WORKDIR /app

# Install dependencies
COPY package.json .

RUN npm install

# Copy source file to /app
COPY . .

# Build solution
RUN npm run build

# Export Port 3000 for external access
EXPOSE 5000

ENV NUXT_HOST=0.0.0.0

ENV NUXT_PORT=5000

CMD ["npm", "start"]
