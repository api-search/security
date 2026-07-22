---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reveliolabs.com
  spf: true
hosts:
- cert_expires: Sep 27 17:53:53 2026 GMT
  host: reveliolabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: www.data-dictionary.reveliolabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.reveliolabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Revelio Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revelio Labs, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revelio Labs
provider_slug: revelio-labs
slug: revelio-labs-domain-security
source_filename: revelio-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reveliolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:53:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.data-dictionary.reveliolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.reveliolabs.com\n  https: false\ndomains:\n- domain: reveliolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revelio-labs/refs/heads/main/security/revelio-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Intelligence
- Labor Market Data
- HR Analytics
- Talent Analytics
- People Analytics
- Data
---
