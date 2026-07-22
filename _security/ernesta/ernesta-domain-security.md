---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ernesta.com
  spf: true
hosts:
- cert_expires: Sep 10 10:57:33 2026 GMT
  host: www.ernesta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ernesta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ernesta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ernesta
provider_slug: ernesta
slug: ernesta-domain-security
source_filename: ernesta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ernesta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 10:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ernesta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ernesta/refs/heads/main/security/ernesta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Rugs
- Home
- Interior Design
- E-commerce
- Retail
- Direct to Consumer
---
