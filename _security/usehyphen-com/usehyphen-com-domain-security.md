---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usehyphen.com
  spf: true
hosts:
- cert_expires: Nov 27 07:42:24 2026 GMT
  host: usehyphen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usehyphen Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyphen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyphen
provider_slug: usehyphen-com
slug: usehyphen-com-domain-security
source_filename: usehyphen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usehyphen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 07:42:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usehyphen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/usehyphen-com/security/usehyphen-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Production
- Kitchen Management
- Order Management
- Inventory Forecasting
- Labor Management
---
