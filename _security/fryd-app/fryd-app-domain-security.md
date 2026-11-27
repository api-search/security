---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fryd.app
  spf: true
hosts:
- cert_expires: Jan 28 09:29:30 2027 GMT
  host: fryd.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fryd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fryd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fryd
provider_slug: fryd-app
slug: fryd-app-domain-security
source_filename: fryd-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fryd.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 09:29:30 2027 GMT\n  hsts: false\ndomains:\n- domain: fryd.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fryd-app/security/fryd-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gardening
- Planting
- Sustainability
- Community
- Premium
---
