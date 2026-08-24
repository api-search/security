---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goodera.com
  spf: true
hosts:
- cert_expires: Nov 10 02:43:07 2026 GMT
  host: www.goodera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: developer-api.goodera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: mcp.goodera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Goodera
provider_slug: goodera
slug: goodera-domain-security
source_filename: goodera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 02:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-api.goodera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: mcp.goodera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goodera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodera/refs/heads/main/security/goodera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Corporate Volunteering
- Social Impact
- CSR
- Employee Engagement
- Nonprofits
- Events
- Volunteering
- ESG
- Model Context Protocol
---
