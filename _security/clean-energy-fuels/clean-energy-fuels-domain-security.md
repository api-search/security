---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cleanenergyfuels.com
  spf: true
hosts:
- cert_expires: Sep  1 18:30:41 2026 GMT
  host: www.cleanenergyfuels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.cleanenergyfuels.com
  https: false
- host: api.cleanenergyfuels.com
  https: false
kind: domain-security
layout: security
method: probed
name: Clean Energy Fuels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clean Energy Fuels, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clean Energy Fuels
provider_slug: clean-energy-fuels
slug: clean-energy-fuels-domain-security
source_filename: clean-energy-fuels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cleanenergyfuels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:30:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cleanenergyfuels.com\n  https: false\n- host: api.cleanenergyfuels.com\n  https: false\ndomains:\n- domain: cleanenergyfuels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clean-energy-fuels/refs/heads/main/security/clean-energy-fuels-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Natural Gas
- Renewable
- Transportation
---
