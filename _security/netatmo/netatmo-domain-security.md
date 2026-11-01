---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: netatmo.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: netatmo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netatmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netatmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Netatmo
provider_slug: netatmo
slug: netatmo-domain-security
source_filename: netatmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netatmo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: netatmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/netatmo/security/netatmo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- SmartHome
- IoT
- Devices
- API
---
