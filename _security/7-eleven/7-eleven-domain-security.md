---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 7-eleven.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.7-eleven.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 7 Eleven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7-Eleven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 7-Eleven
provider_slug: 7-eleven
slug: 7-eleven-domain-security
source_filename: 7-eleven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.7-eleven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 7-eleven.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7-eleven/refs/heads/main/security/7-eleven-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Convenience Stores
---
