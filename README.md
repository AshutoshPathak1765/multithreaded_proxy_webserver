# HTTP Proxy Server with Caching

A high-performance multi-threaded HTTP proxy server with LRU caching, implemented in C.

## Key Features
- 🚀 **Multi-threaded architecture** (handles `MAX_CLIENTS` concurrent connections)
- 💾 **LRU caching** (configurable up to 200MB)
- 🔒 **Thread-safe operations** (mutex-protected cache)
- 📡 **HTTP/1.1 compliant** (GET/POST/HEAD support)
- 📊 **Error handling** (400/403/404/500 responses)

- [Model Link](https://app.eraser.io/workspace/BiyovyJNQf5KDVpC59mM?origin=share)

## Quick Start
```bash
# Compile (requires pthreads)
gcc -pthread proxy.c -o proxy

# Run on port 8080
./proxy 8080

# Test with curl
curl -x http://localhost:8080 http://example.com
