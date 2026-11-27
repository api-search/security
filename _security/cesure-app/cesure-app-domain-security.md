---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cesure.app
  spf: true
hosts:
- cert_expires: Jan  9 22:26:33 2027 GMT
  host: cesure.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cesure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cesure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cesure
provider_slug: cesure-app
slug: cesure-app-domain-security
source_filename: cesure-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cesure.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 22:26:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cesure.app\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cesure-app/security/cesure-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Music
- Guitar
- Artificial Intelligence
- Web App
- Collaboration
---
