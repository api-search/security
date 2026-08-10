---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: verdagy.com
  spf: true
hosts:
- cert_expires: Oct  2 06:01:29 2026 GMT
  host: verdagy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdagy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verdagy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Verdagy
provider_slug: verdagy
slug: verdagy-domain-security
source_filename: verdagy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verdagy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:01:29 2026 GMT\n  hsts: false\ndomains:\n- domain: verdagy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdagy/refs/heads/main/security/verdagy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Clean Energy
- Green Hydrogen
- Hydrogen
- Electrolyzers
- Industrial Equipment
- Manufacturing
- Decarbonization
- Climate Tech
---
