---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: backrest.org
  spf: false
hosts:
- cert_expires: Jan 23 12:00:18 2027 GMT
  host: backrest.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Backrest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backrest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Backrest
provider_slug: backrest
slug: backrest-domain-security
source_filename: backrest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backrest.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:00:18 2027 GMT\n  hsts: false\ndomains:\n- domain: backrest.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/backrest/security/backrest-domain-security.yml
summary_line: TLSv1.3
tags:
- Backup
- Storage
- Restic
- OpenSource
- Go
---
