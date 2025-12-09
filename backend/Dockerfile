# --- Backend Dockerfile ---
FROM node:18-alpine

WORKDIR /app

# Copy package files first (better caching)
COPY package*.json ./

RUN npm install

# Copy source code
COPY . .

# Expose backend port (change if different)
EXPOSE 5000

# Run backend
CMD ["npm", "start"]
