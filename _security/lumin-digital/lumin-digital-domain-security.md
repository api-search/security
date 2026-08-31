---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lumindigital.com
  spf: true
hosts:
- cert_expires: Nov 13 19:25:31 2026 GMT
  host: lumindigital.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumin Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumin Digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lumin Digital
provider_slug: lumin-digital
slug: lumin-digital-domain-security
source_filename: lumin-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumindigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 19:25:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lumindigital.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumin-digital/refs/heads/main/security/lumin-digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Digital Banking
- Banking
- Credit Unions
- Financial-Services
- Fintech
- Core Banking
- Digital Account Opening
- Payments
- Commercial Banking
- Software-as-a-Service
---
