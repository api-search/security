---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: k2view.com
  spf: true
hosts:
- cert_expires: Nov 19 14:17:24 2026 GMT
  host: www.k2view.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: K2View Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for K2view, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: K2view
provider_slug: k2view
slug: k2view-domain-security
source_filename: k2view-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.k2view.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 14:17:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: k2view.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/k2view/refs/heads/main/security/k2view-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- Data Platform
- AI
- Enterprise
---
