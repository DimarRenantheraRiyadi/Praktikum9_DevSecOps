# Praktikum 9 DevSecOps - Container Security

Repository ini dibuat untuk memenuhi Tugas Praktikum Pertemuan 9 (Container Security).

## Fitur Keamanan:
- Menggunakan Multi-stage Build di Dockerfile.
- Menjalankan container sebagai non-root user (`appuser`).
- Menggunakan base image minimal (`python:3.12-alpine`).
- Integrasi Trivy Vulnerability Scanner via GitHub Actions.

## Cara Menjalankan Aplikasi:
1. Build image: `docker build -f Dockerfile.secure -t my-app:v1 .`
2. Jalankan container: `docker run -p 8080:8080 my-app:v1`