---
description: ''
domains:
- caa:
  - 0 issue "DigiCert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microbilt.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.microbilt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ibvnow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microbilt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microbilt
provider_slug: ibvnow
slug: ibvnow-domain-security
source_filename: ibvnow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microbilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microbilt.com\n  dnssec: false\n  caa:\n  - 0 issue \"DigiCert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ibvnow/security/ibvnow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Credit
- RiskManagement
- APIs
---
