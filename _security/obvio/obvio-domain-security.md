---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: obvio.ai
  spf: false
hosts:
- cert_expires: Oct 18 03:37:59 2026 GMT
  host: www.obvio.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Obvio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obvio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Obvio
provider_slug: obvio
slug: obvio-domain-security
source_filename: obvio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.obvio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:37:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: obvio.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obvio/refs/heads/main/security/obvio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Ai
- Traffic Safety
- Public Safety
- Computer Vision
- Road Safety
- Law Enforcement
- Artificial Intelligence
---
