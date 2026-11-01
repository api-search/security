---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smartenergy.at
  spf: true
hosts:
- cert_expires: Dec 10 21:07:05 2026 GMT
  host: smartenergy.at
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smartenergy At Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for smartENERGY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: smartENERGY
provider_slug: smartenergy-at
slug: smartenergy-at-domain-security
source_filename: smartenergy-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartenergy.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 21:07:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smartenergy.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/smartenergy-at/security/smartenergy-at-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Renewable
- SmartGrid
- API
- Austria
---
