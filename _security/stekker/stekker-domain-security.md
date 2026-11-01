---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stekker.com
  spf: true
hosts:
- cert_expires: Dec  4 18:47:58 2026 GMT
  host: stekker.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stekker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stekker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stekker
provider_slug: stekker
slug: stekker-domain-security
source_filename: stekker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stekker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 18:47:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: stekker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/stekker/security/stekker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- EV
- Renewable
- Marketplace
- Netherlands
---
