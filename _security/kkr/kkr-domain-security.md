---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kkr.com
  spf: true
hosts:
- cert_expires: Aug 18 03:48:14 2026 GMT
  host: www.kkr.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kkr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KKR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KKR
provider_slug: kkr
slug: kkr-domain-security
source_filename: kkr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kkr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:48:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: kkr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kkr/refs/heads/main/security/kkr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Private Equity
- Asset Management
- Investment
- Finance
---
