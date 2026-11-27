---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: clepit.com
  spf: false
hosts:
- cert_expires: Jan 30 11:56:41 2027 GMT
  host: clepit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clepit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clepit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Clepit
provider_slug: clepit-com
slug: clepit-com-domain-security
source_filename: clepit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clepit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 11:56:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clepit.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/clepit-com/security/clepit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Block Editor
- Rich Text Editor
- Knowledge Base
- Open Source
- TypeScript
- JSON
- Collaboration
- Wiki
---
