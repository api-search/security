---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catalent.com
  spf: true
hosts:
- cert_expires: Aug 20 20:15:56 2026 GMT
  host: www.catalent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.catalent.com
  https: false
- host: api.catalent.com
  https: false
kind: domain-security
layout: security
method: probed
name: Catalent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalent, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Catalent
provider_slug: catalent
slug: catalent-domain-security
source_filename: catalent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.catalent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 20:15:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.catalent.com\n  https: false\n- host: api.catalent.com\n  https: false\ndomains:\n- domain: catalent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catalent/refs/heads/main/security/catalent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharmaceutical Services
- Drug Delivery
---
