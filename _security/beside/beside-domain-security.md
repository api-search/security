---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beside.com
  spf: true
hosts:
- cert_expires: Aug 17 16:15:19 2026 GMT
  host: www.beside.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beside, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beside
provider_slug: beside
slug: beside-domain-security
source_filename: beside-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beside.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:15:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beside.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beside/refs/heads/main/security/beside-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software
- Communications
- Voice
- Artificial Intelligence
- Receptionist
- Telephony
- SMB
- CRM
---
