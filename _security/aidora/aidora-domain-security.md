---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getaidora.com
  spf: true
hosts:
- cert_expires: Oct 21 19:02:03 2026 GMT
  host: www.getaidora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aidora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aidora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aidora
provider_slug: aidora
slug: aidora-domain-security
source_filename: aidora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getaidora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 19:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getaidora.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidora/refs/heads/main/security/aidora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Human Resources
- Leave Management
- Absence Management
- HR Compliance
- Workforce
- Artificial Intelligence
- Software-as-a-Service
- Acquired
---
