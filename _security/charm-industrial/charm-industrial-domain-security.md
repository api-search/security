---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charmindustrial.com
  spf: true
hosts:
- cert_expires: Sep 16 11:53:31 2026 GMT
  host: charmindustrial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charm Industrial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charm Industrial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Charm Industrial
provider_slug: charm-industrial
slug: charm-industrial-domain-security
source_filename: charm-industrial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charmindustrial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:53:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: charmindustrial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charm-industrial/refs/heads/main/security/charm-industrial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Carbon Removal
- Climate Tech
- Carbon Dioxide Removal
- Bio-oil
- Pyrolysis
- Sustainability
- Sequestration
---
