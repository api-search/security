---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: redis.io
  spf: true
hosts:
- cert_expires: Oct  5 19:28:48 2026 GMT
  host: redis.io
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redis Streams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redis Streams, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Redis Streams
provider_slug: redis-streams
slug: redis-streams-domain-security
source_filename: redis-streams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:28:48 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\ndomains:\n- domain: redis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redis-streams/refs/heads/main/security/redis-streams-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Groups
- Event-Driven
- In-Memory
- Messaging
- Redis
- Streaming
---
