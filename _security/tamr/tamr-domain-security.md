---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tamr.com
  spf: true
hosts:
- cert_expires: Aug 20 23:25:26 2026 GMT
  host: www.tamr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:31:15 2026 GMT
  host: docs.tamr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tamr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tamr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tamr
provider_slug: tamr
slug: tamr-domain-security
source_filename: tamr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tamr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tamr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:31:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tamr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamr/refs/heads/main/security/tamr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Management
- Machine Learning
- Enterprise Software
- Master Data Management
---
