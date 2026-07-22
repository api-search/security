---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greenboard.com
  spf: true
hosts:
- cert_expires: Sep 16 07:30:00 2026 GMT
  host: www.greenboard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Greenboard
provider_slug: greenboard
slug: greenboard-domain-security
source_filename: greenboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greenboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:30:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: greenboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenboard/refs/heads/main/security/greenboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- RegTech
- Financial Services
- SEC
- FINRA
- Communications Archiving
- Governance
- Risk
- Artificial Intelligence
---
