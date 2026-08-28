---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quaise.com
  spf: true
hosts:
- cert_expires: Nov 19 08:01:00 2026 GMT
  host: www.quaise.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quaise Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quaise Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quaise Energy
provider_slug: quaise-energy
slug: quaise-energy-domain-security
source_filename: quaise-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quaise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 08:01:00 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: quaise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaise-energy/refs/heads/main/security/quaise-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Geothermal
- Clean Energy
- Drilling
- Deep Tech
- Climate Tech
- Hardware
---
