# DevContainer per sviluppo locale identico a GitHub Actions
FROM ubuntu:22.04

# Evita domande interattive
ENV DEBIAN_FRONTEND=noninteractive

# Installa dipendenze di sistema
RUN apt-get update && \
    apt-get install -y curl wget git ca-certificates build-essential gnupg lsb-release unzip && \
    rm -rf /var/lib/apt/lists/*

# Installa Go (necessario per hugo modules)
ENV GO_VERSION=1.22.3
RUN wget https://go.dev/dl/go${GO_VERSION}.linux-amd64.tar.gz && \
    tar -C /usr/local -xzf go${GO_VERSION}.linux-amd64.tar.gz && \
    rm go${GO_VERSION}.linux-amd64.tar.gz
ENV PATH="/usr/local/go/bin:${PATH}"

# Installa Node.js (LTS) e npm
RUN curl -fsSL https://deb.nodesource.com/setup_lts.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g npm@latest


# Installa Hugo extended (sceglie architettura corretta)
ENV HUGO_VERSION=0.136.5
RUN ARCH=$(uname -m) && \
        if [ "$ARCH" = "x86_64" ]; then \
            HUGO_ARCH=amd64; \
        elif [ "$ARCH" = "aarch64" ] || [ "$ARCH" = "arm64" ]; then \
            HUGO_ARCH=arm64; \
        else \
            echo "Unsupported architecture: $ARCH" && exit 1; \
        fi && \
        wget -O hugo.tar.gz https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_extended_${HUGO_VERSION}_linux-${HUGO_ARCH}.tar.gz && \
        tar -xzvf hugo.tar.gz -C /usr/local/bin hugo && \
        rm hugo.tar.gz

# Installa pagefind come dipendenza globale (opzionale, ma utile per debug)
RUN npm install -g pagefind

# Crea utente non-root per VS Code
RUN useradd -m vscode
USER vscode
WORKDIR /workspace

# Consigliato: copia package.json/package-lock.json se presenti per caching
# COPY package*.json ./
# RUN npm install

# Esporta porta per hugo server
EXPOSE 1313
