![logo](https://eliasdh.com/assets/media/images/logo-github.png)
# 💙🤍Setup Secrets🤍💙

## 📘Table of Contents

1. [📘Table of Contents](#📘table-of-contents)
2. [🖖Introduction](#🖖introduction)
3. [✨Steps](#✨steps)
    1. [👉Step 1: Create a GitHub Secrets](#👉step-1-create-a-github-secrets)
    2. [👉Step 2: Create a GitHub Secrets](#👉step-2-create-a-github-secrets)
4. [🔗Links](#🔗links)

---

## 🖖Introduction

This document provides a step-by-step guide to setting up `Kubernetes Secrets` on the servers (nodes) in the supercluster. The steps outlined in this document are essential for ensuring the proper functioning of the servers (nodes) and the supercluster.

## ✨Steps

### 👉Step 1: Create a GitHub Secrets

```bash
kubectl create secret docker-registry github-registry \
  --docker-server=ghcr.io \
  --docker-username=<username> \
  --docker-password=<access_token> \
  --docker-email=<email> \
  --namespace=default
```

### 👉Step 2: Create a GitHub Secrets

```bash
kubectl create secret docker-registry gitlab-registry \
    --docker-server=registry.gitlab.com \
    --docker-username=<username> \
    --docker-password=<access_token> \
    --docker-email=<email> \
    --namespace=default
```

## 🔗Links
- 👯 Web hosting company [EliasDH.com](https://eliasdh.com).
- 📫 How to reach us elias.dehondt@outlook.com