sequenceDiagram
  participant k as Key Program
  participant fs as File System
  participant c as Authenticated Secrets Consumers
  k->>fs: Read Master Key files and timestamp partials
  fs-->>k: Derive Master Key (KEK)
  k->>fs: Read KEK(DEK)
  k->>k: Decrypt DEK with KEK

  c->>k: Secret(key)
  k-->>c: Secret
