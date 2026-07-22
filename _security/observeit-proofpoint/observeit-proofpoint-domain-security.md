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
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.proofpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Observeit Proofpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ObserveIT (Proofpoint), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ObserveIT (Proofpoint)
provider_slug: observeit-proofpoint
slug: observeit-proofpoint-domain-security
source_filename: observeit-proofpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proofpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: proofpoint.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodo.com\"\n  - 0 issue \"thawte.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observeit-proofpoint/refs/heads/main/security/observeit-proofpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Infrastructure
- Security
- Insider Threat Management
- Data Loss Prevention
- Cybersecurity
- Endpoint Monitoring
- Proofpoint
---
