---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lobster.ist
  spf: true
hosts:
- cert_expires: May  5 23:59:59 2027 GMT
  host: lobster.ist
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lobster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lobster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lobster
provider_slug: lobster-ist
slug: lobster-ist-domain-security
source_filename: lobster-ist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lobster.ist\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lobster.ist\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lobster-ist/security/lobster-ist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Public Affairs
- CRM
- Lobbying
- GDPR
- CSRD
---
