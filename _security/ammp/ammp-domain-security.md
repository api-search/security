---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ammp.io
  spf: true
hosts:
- cert_expires: Sep  3 13:33:56 2026 GMT
  host: www.ammp.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ammp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMMP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AMMP
provider_slug: ammp
slug: ammp-domain-security
source_filename: ammp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ammp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 13:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ammp.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ammp/refs/heads/main/security/ammp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Solar
- Energy
- Renewable Energy
- Monitoring
- Asset Management
- Battery Storage
- IoT
- Clean Energy
---
