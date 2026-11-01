---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: i2dev.com
  spf: true
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: i2dev.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: I2Dev Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for i2dev-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: i2dev-com
provider_slug: i2dev-com
slug: i2dev-com-domain-security
source_filename: i2dev-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: i2dev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: i2dev.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/i2dev-com/security/i2dev-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DeveloperTools
- VisualRegression
- CI
- OpenSource
- SaaS
---
