---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spideroak.com
  spf: true
hosts:
- cert_expires: Nov  3 20:11:08 2026 GMT
  host: spideroak.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spideroak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpiderOak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpiderOak
provider_slug: spideroak
slug: spideroak-domain-security
source_filename: spideroak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spideroak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 20:11:08 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: spideroak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spideroak/refs/heads/main/security/spideroak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Zero Trust
- Encryption
- Access Control
- Identity and Access Management
- Cryptography
- Defense
- Aerospace
- Space
- Open Source
- Edge Computing
- Data Exchange
- Backup and Storage
---
