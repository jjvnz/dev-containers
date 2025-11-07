# Development Containers 🐳

Ready-to-use Docker Compose configurations for local development environments.

## 🚀 Quick Start

```bash
# PostgreSQL
docker-compose -f docker-compose-postgres.yml up -d

# MongoDB
docker-compose -f docker-compose-mongo.yml up -d

# Redis
docker-compose -f docker-compose-redis.yml up -d

# Kafka
docker-compose -f docker-compose-kafka.yml up -d
```

## 📦 Available Services

| Service | Port | Use Case |
|---------|------|----------|
| PostgreSQL | 5432 | Relational data, transactions |
| MongoDB | 27017 | Document storage, flexible schemas |
| Redis | 6379 | Caching, sessions, real-time data |
| Kafka | 9092 | Event streaming, message queues |

## 🛠 Development Usage

### For Backend Development:
```bash
# Start dependencies for a microservice
docker-compose -f docker-compose-postgres.yml -f docker-compose-redis.yml up -d
```

### For Local Testing:
```bash
# Stop all services
docker-compose -f docker-compose-*.yml down

# View logs
docker-compose -f docker-compose-postgres.yml logs -f
```

## 🔧 Configuration Examples

Each service includes:
- **Persistent volumes** for data preservation
- **Environment variables** for easy configuration
- **Network setup** for multi-service communication

## 📚 Ideal For
- Local development environments
- CI/CD pipeline testing
- Microservices architecture prototyping
- Database testing and experimentation

---

**Maintained by:** [Jair Villalobos](https://github.com/jlynz) | Backend Engineer
