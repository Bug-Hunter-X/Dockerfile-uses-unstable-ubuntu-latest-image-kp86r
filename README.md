# Dockerfile Best Practices

This repository demonstrates a common mistake in Dockerfiles: using the `ubuntu:latest` image. This can lead to inconsistencies and unexpected behavior in your Docker builds.

## Problem

Using `ubuntu:latest` means your Dockerfile relies on the latest version of Ubuntu, which can change at any time. This means that your build might work today, but fail tomorrow if a new version of Ubuntu introduces breaking changes.

## Solution

Always specify a particular Ubuntu version in your Dockerfile (e.g., `ubuntu:20.04`). This ensures that your build is reproducible and avoids unexpected issues.