---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atmosenergy.com
  spf: true
hosts:
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: www.atmosenergy.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Atmos Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmos Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atmos Energy
provider_slug: atmos-energy
slug: atmos-energy-domain-security
source_filename: atmos-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atmosenergy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: atmosenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmos-energy/refs/heads/main/security/atmos-energy-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Energy
- Natural Gas
- Utilities
- Infrastructure
- Fortune 1000
---
