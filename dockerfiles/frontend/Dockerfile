FROM node:24.11.0-alpine

WORKDIR /frontend

# pnpmのグローバルディレクトリ設定
ENV PNPM_HOME="/pnpm"
ENV PATH="$PNPM_HOME:$PATH"

# Corepackの有効化
RUN corepack enable

# Claude Code のインストール
RUN pnpm add -g @anthropic-ai/claude-code

RUN apk add --no-cache \
  bash

ENV SHELL=/bin/bash