---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doxa.app
  spf: true
hosts:
- cert_expires: Dec  6 16:09:43 2026 GMT
  host: doxa.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doxa App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doxa-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: doxa-app
provider_slug: doxa-app
slug: doxa-app-domain-security
source_filename: doxa-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doxa.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 16:09:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: doxa.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/doxa-app/security/doxa-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Faith
- Community
- MobileApp
- BibleResources
- Prophetic
---
