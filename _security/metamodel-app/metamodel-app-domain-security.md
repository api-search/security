---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metamodel.app
  spf: true
hosts:
- cert_expires: Jan 27 16:03:57 2027 GMT
  host: metamodel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MetaModel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MetaModel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MetaModel
provider_slug: metamodel-app
slug: metamodel-app-domain-security
source_filename: metamodel-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metamodel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 16:03:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: metamodel.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/metamodel-app/security/metamodel-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Engineering
- Manufacturing
- Quoting
- Configurator
---
