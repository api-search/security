---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: manpower.com
  spf: true
hosts:
- cert_expires: Sep 20 20:12:14 2026 GMT
  host: www.manpower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manpower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Manpower
provider_slug: manpower
slug: manpower-domain-security
source_filename: manpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.manpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:12:14 2026 GMT\n  hsts: false\ndomains:\n- domain: manpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manpower/refs/heads/main/security/manpower-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Workforce
- Staffing
- Talent
- Human Resources
- Fortune 500
---
