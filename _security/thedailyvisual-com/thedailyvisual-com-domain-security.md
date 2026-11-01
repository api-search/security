---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thedailyvisual.com
  spf: false
hosts:
- cert_expires: Jan 22 19:38:59 2027 GMT
  host: thedailyvisual.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thedailyvisual Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Daily Visual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: The Daily Visual
provider_slug: thedailyvisual-com
slug: thedailyvisual-com-domain-security
source_filename: thedailyvisual-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thedailyvisual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 19:38:59 2027 GMT\n  hsts: false\ndomains:\n- domain: thedailyvisual.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thedailyvisual-com/security/thedailyvisual-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Visualizations
- Climate
- Economics
---
