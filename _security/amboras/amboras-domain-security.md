---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: amboras.com
  spf: true
hosts:
- cert_expires: Sep  2 20:38:42 2026 GMT
  host: www.amboras.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amboras Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amboras, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Amboras
provider_slug: amboras
slug: amboras-domain-security
source_filename: amboras-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amboras.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:38:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amboras.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amboras/refs/heads/main/security/amboras-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-Commerce
- AI
- Generative AI
- Automation
- Conversion Rate Optimization
- Retail
- No-Code Store Builder
- Y Combinator
---
