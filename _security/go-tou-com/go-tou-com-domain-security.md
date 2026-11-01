---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: go-tou.com
  spf: true
hosts:
- cert_expires: Apr 19 23:59:59 2027 GMT
  host: go-tou.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Go Tou Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go To-U, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Go To-U
provider_slug: go-tou-com
slug: go-tou-com-domain-security
source_filename: go-tou-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: go-tou.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: go-tou.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/go-tou-com/security/go-tou-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- EV
- Charging
- Platform
- SaaS
- CPO
---
