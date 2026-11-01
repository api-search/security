---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noddle.dev
  spf: false
hosts:
- cert_expires: Dec 26 12:33:21 2026 GMT
  host: noddle.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Noddle Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for noddle-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: noddle-dev
provider_slug: noddle-dev
slug: noddle-dev-domain-security
source_filename: noddle-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noddle.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:33:21 2026 GMT\n  hsts: false\ndomains:\n- domain: noddle.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/noddle-dev/security/noddle-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Platform
- API Management
- Web Development
- Cloud Services
---
