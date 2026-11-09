---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: adminlanding.com
  spf: true
hosts:
- cert_expires: Jan 10 00:04:36 2027 GMT
  host: adminlanding.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adminlanding Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdminLanding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AdminLanding
provider_slug: adminlanding-com
slug: adminlanding-com-domain-security
source_filename: adminlanding-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adminlanding.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 00:04:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adminlanding.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adminlanding-com/security/adminlanding-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software-as-a-Service
- French Administration
- Real Estate
- Tax
---
