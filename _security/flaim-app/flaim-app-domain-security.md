---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flaim.app
  spf: true
hosts:
- cert_expires: Jan 11 18:47:07 2027 GMT
  host: flaim.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flaim Fantasy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flaim Fantasy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flaim Fantasy
provider_slug: flaim-app
slug: flaim-app-domain-security
source_filename: flaim-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flaim.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 18:47:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flaim.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flaim-app/security/flaim-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fantasy Sports
- Artificial Intelligence
- ChatGPT
- ESPN
---
