---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: genesisenergy.com
  spf: true
hosts:
- cert_expires: Dec  7 11:29:07 2026 GMT
  host: www.genesisenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Genesis Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Genesis Energy
provider_slug: genesis-energy
slug: genesis-energy-domain-security
source_filename: genesis-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genesisenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 11:29:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genesisenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesis-energy/refs/heads/main/security/genesis-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Midstream
- Oil and Gas
- Pipelines
- Natural Gas
- Crude Oil
- Marine Transportation
- Soda Ash
---
