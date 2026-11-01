---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "telesec.de"
  - 0 issuewild "digicert.com"
  - 0 issue "Digicert.com"
  - 0 issuewild "telesec.de"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gmx.net
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: gmx.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gmx Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GMX (mail), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: GMX (mail)
provider_slug: gmx-net
slug: gmx-net-domain-security
source_filename: gmx-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gmx.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gmx.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"telesec.de\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"Digicert.com\"\n  - 0 issuewild \"telesec.de\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gmx-net/security/gmx-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Cloud
- Free
- German
---
