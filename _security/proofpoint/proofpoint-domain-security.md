---
description: ''
domains:
- caa:
  - 0 issue "comodo.com"
  - 0 issue "thawte.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: proofpoint.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: help.proofpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: tap-api-v2.proofpoint.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: threatprotection-api.proofpoint.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Proofpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proofpoint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Proofpoint
provider_slug: proofpoint
slug: proofpoint-domain-security
source_filename: proofpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.proofpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tap-api-v2.proofpoint.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: threatprotection-api.proofpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: proofpoint.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodo.com\"\n  - 0 issue \"thawte.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proofpoint/refs/heads/main/security/proofpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Cybersecurity
- Email Security
- Threat Intelligence
- Data Loss Prevention
- Security Awareness Training
- Insider Threat
- SIEM
- Compliance
- Email
---
