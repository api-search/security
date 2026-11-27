---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bciseguros.cl
  spf: true
hosts:
- cert_expires: Jan  3 14:19:52 2027 GMT
  host: www.bciseguros.cl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BCI Seguros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BCI Seguros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BCI Seguros
provider_slug: bciseguros
slug: bciseguros-domain-security
source_filename: bciseguros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bciseguros.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 14:19:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bciseguros.cl\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bciseguros/security/bciseguros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Chile
- Auto
- Homes
- Health
---
