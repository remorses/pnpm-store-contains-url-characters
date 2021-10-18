Repro

When installing a package from an url, pnpm creates a directory using url character like `?` that will fail with many resolve implementations like `enhanced-resolve`


To reproduce
```
cd pnpm
pnpm install
ls pnpm/node_modules/.pnpm/@gitpkg.now.sh+remorses+genql@runtime?4e431e1a6e2cea513cad91614f3a9ef794f94d07
```