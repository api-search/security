---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:security@astrus.ai"
  - 0 issue "sectigo.com"
  - 0 issuewild ";"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astrus.ai
  spf: true
hosts:
- cert_expires: Aug 23 00:42:58 2026 GMT
  host: www.astrus.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astrus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astrus
provider_slug: astrus
slug: astrus-domain-security
source_filename: astrus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astrus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:42:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: astrus.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:security@astrus.ai\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrus/refs/heads/main/security/astrus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Semiconductors
- Chip Design
- Electronic Design Automation
- Analog Circuits
- Machine Learning
- Reinforcement Learning
---
