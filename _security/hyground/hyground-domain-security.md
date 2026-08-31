---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hyground.ai
  spf: true
hosts:
- cert_expires: Sep 27 14:13:08 2026 GMT
  host: hyground.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyground Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyground, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hyground
provider_slug: hyground
slug: hyground-domain-security
source_filename: hyground-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyground.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:13:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hyground.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyground/refs/heads/main/security/hyground-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai/Ml
- Site Reliability Engineering
- DevOps
- Kubernetes
- Incident Response
- Observability
- AIOps
- Compliance
- Europe
---
