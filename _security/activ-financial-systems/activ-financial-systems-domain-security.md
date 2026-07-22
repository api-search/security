---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: activfinancial.com
  spf: true
hosts:
- cert_expires: Oct 11 18:00:06 2026 GMT
  host: www.activfinancial.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Activ Financial Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACTIV Financial Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ACTIV Financial Systems
provider_slug: activ-financial-systems
slug: activ-financial-systems-domain-security
source_filename: activ-financial-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: activfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activ-financial-systems/refs/heads/main/security/activ-financial-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Market Data
- Financial Data
- Real-Time Data
- Trading Infrastructure
- Options Technology
---
