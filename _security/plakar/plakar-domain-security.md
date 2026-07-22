---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plakar.io
  spf: true
hosts:
- cert_expires: Aug 15 13:04:19 2026 GMT
  host: plakar.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plakar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plakar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plakar
provider_slug: plakar
slug: plakar-domain-security
source_filename: plakar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plakar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 13:04:19 2026 GMT\n  hsts: false\ndomains:\n- domain: plakar.io\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plakar/refs/heads/main/security/plakar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Backup
- Data Protection
- Disaster Recovery
- Open Source
- Encryption
- Deduplication
- Storage
- CLI
- gRPC
- Go SDK
- Kubernetes
---
