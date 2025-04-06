# 🐘 postgres-dock

A minimal, no-nonsense setup for running PostgreSQL in Docker. No magic, just containers.

## 🧱 What's Inside

- PostgreSQL 16 running in a Docker container
- `docker-compose.yml` to keep things civilized
- Optional `init.sql` for those who like their databases pre-seasoned

## 🚀 Quick Start

1. Clone this repo (you knew that).
2. Spin up the container:

   ```bash
   docker-compose up -d 
   ```
3. Connect using your favorite SQL client:
    ```bash
    Host:     localhost
    Port:     5432
    User:     admin
    Password: password123
    DB Name:  mydb
    ```

## 📂 Structure
```bash
/postgres-dock
├── docker-compose.yml      # spins up the goods
├── Dockerfile.postgres     # (optional) custom image logic
└── init.sql                # (optional) schema & seed
```

## 🧼 Cleanup
Done playing God with your data?
```bash
docker-compose down -v
```
