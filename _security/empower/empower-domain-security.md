---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: empower.com
  spf: true
hosts:
- cert_expires: Nov 16 13:35:09 2026 GMT
  host: www.empower.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Empower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Empower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Empower
provider_slug: empower
slug: empower-domain-security
source_filename: empower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.empower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 13:35:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: empower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empower/refs/heads/main/security/empower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Investment
- Retirement
- Financial-Tools
---
