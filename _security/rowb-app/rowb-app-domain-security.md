---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rowb.app
  spf: true
hosts:
- cert_expires: Jan  7 16:37:28 2027 GMT
  host: rowb.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rowb App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rowb-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: rowb-app
provider_slug: rowb-app
slug: rowb-app-domain-security
source_filename: rowb-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rowb.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:37:28 2027 GMT\n  hsts: false\ndomains:\n- domain: rowb.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rowb-app/security/rowb-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Tools
- Deterministic
- No-Auth
---
