---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: maltamprp.com
  spf: false
hosts:
- cert_expires: Jan 31 14:56:42 2027 GMT
  host: maltamprp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Malta MPRP Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Malta MPRP Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Malta MPRP Guide
provider_slug: maltamprp-com
slug: maltamprp-com-domain-security
source_filename: maltamprp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maltamprp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 14:56:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maltamprp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/maltamprp-com/security/maltamprp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Residency
- Investment
- Malta
- guide
- Permanent-Residence
---
