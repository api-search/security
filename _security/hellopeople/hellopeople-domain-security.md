---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild ";"
  - 0 iodef "mailto:info@hellopeople.com.au"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hellopeople.com.au
  spf: true
hosts:
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: hellopeople.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hellopeople Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HELLO PEOPLE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HELLO PEOPLE
provider_slug: hellopeople
slug: hellopeople-domain-security
source_filename: hellopeople-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hellopeople.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hellopeople.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:info@hellopeople.com.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hellopeople/security/hellopeople-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Integration
- Automation
- Software
---
