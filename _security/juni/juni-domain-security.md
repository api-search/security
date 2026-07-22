---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juni.co
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.juni.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Juni
provider_slug: juni
slug: juni-domain-security
source_filename: juni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.juni.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: juni.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juni/refs/heads/main/security/juni-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Banking
- Spend Management
- Payments
- Ecommerce
- Corporate Cards
- Open Banking
- Sweden
---
