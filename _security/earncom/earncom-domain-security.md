---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: earn.com
  spf: true
hosts:
- cert_expires: Aug 25 09:03:51 2026 GMT
  host: earn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earncom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earn.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Earn.com
provider_slug: earncom
slug: earncom-domain-security
source_filename: earncom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:03:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: earn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earncom/refs/heads/main/security/earncom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Bitcoin
- Payments
- Acquired
- Defunct
- Messaging
---
