version: '3.8'
services:
  backend:
    build:
      context: .
      dockerfile: Dockerfile
    ports:
      - 8001:5000
    volumes:
        - .:/app