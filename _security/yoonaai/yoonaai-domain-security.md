---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yoona.ai
  spf: true
hosts:
- cert_expires: Sep 15 08:37:16 2026 GMT
  host: yoona.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yoonaai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoona.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yoona.ai
provider_slug: yoonaai
slug: yoonaai-domain-security
source_filename: yoonaai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yoona.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:37:16 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: yoona.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoonaai/refs/heads/main/security/yoonaai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Fashion
- Product Design
- Generative AI
- E-Commerce
- Retail
- Product Lifecycle Management
---
