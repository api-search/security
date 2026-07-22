---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buckeye.com
  spf: true
hosts:
- cert_expires: Sep 25 02:55:06 2026 GMT
  host: www.buckeye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buckeye Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buckeye Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Buckeye Partners
provider_slug: buckeye-partners
slug: buckeye-partners-domain-security
source_filename: buckeye-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buckeye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:55:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buckeye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buckeye-partners/refs/heads/main/security/buckeye-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Fuel Storage
- Infrastructure
- Petroleum
- Pipelines
- Refined Products
- Terminals
---
