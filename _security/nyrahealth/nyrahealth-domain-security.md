---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nyra.health
  spf: true
hosts:
- cert_expires: Nov 22 13:26:06 2026 GMT
  host: www.nyra.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nyrahealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NyraHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NyraHealth
provider_slug: nyrahealth
slug: nyrahealth-domain-security
source_filename: nyrahealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nyra.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 13:26:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nyra.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nyrahealth/security/nyrahealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Neurotherapy
- DigitalHealth
- Healthcare
---
