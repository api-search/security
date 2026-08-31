---
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tailor.tech
  spf: true
hosts:
- cert_expires: Sep 17 19:23:22 2026 GMT
  host: www.tailor.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:47:19 2026 GMT
  host: docs.tailor.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:23:22 2026 GMT
  host: api.tailor.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tailor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tailor
provider_slug: tailor
slug: tailor-domain-security
source_filename: tailor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tailor.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:23:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tailor.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:47:19 2026 GMT\n  hsts: false\n- host: api.tailor.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:23:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tailor.tech\n  dnssec: true\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailor/refs/heads/main/security/tailor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- ERP
- Headless ERP
- Retail
- E-Commerce
- Supply Chain
- Inventory Management
- GraphQL
- gRPC
- Low-Code
- Composable Commerce
- Manufacturing
---
