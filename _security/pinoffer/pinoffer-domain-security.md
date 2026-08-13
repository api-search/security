---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: convertedin.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: converted.in
  spf: true
hosts:
- cert_expires: Oct 14 16:32:53 2026 GMT
  host: convertedin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 05:05:23 2026 GMT
  host: developer.converted.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:54:59 2026 GMT
  host: app.converted.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinoffer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinoffer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pinoffer
provider_slug: pinoffer
slug: pinoffer-domain-security
source_filename: pinoffer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convertedin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:32:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.converted.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:05:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.converted.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:54:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: convertedin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: converted.in\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinoffer/refs/heads/main/security/pinoffer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Advertising Technology
- Marketing Technology
- E-commerce
- Marketing Automation
- Customer Data
- Lead Generation
- Payments
- Emerging Markets
- MENA
- Advertising
- Webhooks
---
