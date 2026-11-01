---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: basenull.com
  spf: true
hosts:
- cert_expires: Jan 26 04:06:10 2027 GMT
  host: basenull.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Basenull Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for basenull-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: basenull-com
provider_slug: basenull-com
slug: basenull-com-domain-security
source_filename: basenull-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basenull.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 04:06:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: basenull.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/basenull-com/security/basenull-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- API
- Null-Handling
- DeveloperTools
---
