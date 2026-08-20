---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klarys.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: klarys.app
  spf: true
hosts:
- cert_expires: Oct 18 18:48:05 2026 GMT
  host: www.klarys.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 19:02:06 2026 GMT
  host: klarys.app
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klarys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klarys, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Klarys
provider_slug: klarys
slug: klarys-domain-security
source_filename: klarys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klarys.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 18:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: klarys.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 19:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 60\ndomains:\n- domain: klarys.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: klarys.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarys/refs/heads/main/security/klarys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Software-as-a-Service
- eProcurement
- Procurement
- Supply Chain
- Food and Beverage
- Seafood
- Fresh Food
- Retail
- EDI
- Invoicing
- France
---
