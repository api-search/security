---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ctera.com
  spf: true
hosts:
- cert_expires: Aug 20 14:01:59 2026 GMT
  host: www.ctera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ctera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CTERA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CTERA
provider_slug: ctera
slug: ctera-domain-security
source_filename: ctera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ctera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:01:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ctera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctera/refs/heads/main/security/ctera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Storage
- File Storage
- Global File System
- Data Management
- Edge Computing
- Cyber Protection
- Hybrid Cloud
- Unstructured Data
---
