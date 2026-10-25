---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qube.com.au
  spf: true
hosts:
- cert_expires: Dec 17 00:33:26 2026 GMT
  host: qube.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qube Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qube Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qube Holdings
provider_slug: qube-holdings
slug: qube-holdings-domain-security
source_filename: qube-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qube.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 00:33:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qube.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qube-holdings/refs/heads/main/security/qube-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Ports
- Stevedoring
- Supply Chain
- Freight
- Australia
- Transportation
---
