FROM node:18-alpine

WORKDIR /app

# Copy package files
COPY packages/mcp-server/package*.json ./

# Install dependencies
RUN npm install --production --legacy-peer-deps

# Copy source code
COPY packages/mcp-server/ ./

# Expose port
EXPOSE 3000

# Start server
CMD ["npm", "start"]