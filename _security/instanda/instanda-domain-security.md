---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instanda.com
  spf: true
hosts:
- cert_expires: Sep 18 17:29:44 2026 GMT
  host: instanda.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INSTANDA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: INSTANDA
provider_slug: instanda
slug: instanda-domain-security
source_filename: instanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instanda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:29:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instanda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instanda/refs/heads/main/security/instanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Policy Administration
- Underwriting
- Claims
- Property and Casualty
- Life Insurance
- Health Insurance
- Digital Distribution
- No-Code
- Core Systems
- MGA
- Brokers
- Webhook
- Microsoft Azure
- Embedded Insurance
---
