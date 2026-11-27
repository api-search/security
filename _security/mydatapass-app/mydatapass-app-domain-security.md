---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mydatapass.app
  spf: true
hosts:
- cert_expires: Dec 31 13:25:09 2026 GMT
  host: mydatapass.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyDataPass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyDataPass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MyDataPass
provider_slug: mydatapass-app
slug: mydatapass-app-domain-security
source_filename: mydatapass-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mydatapass.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:25:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mydatapass.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mydatapass-app/security/mydatapass-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Compliance
- Data Management
- Software-as-a-Service
- EU-Regulation
- Privacy
---
