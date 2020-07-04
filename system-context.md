flowchart TB
  sc(Secrets Consumers) -->|"Secret(key)"| mkv(Master Key Vault)
  mkv -->|Secret| sc
  mkv -->|Backup| ol(Offline Storage)
  mkv <-->|Init & System Startup| fs[(File System)]
