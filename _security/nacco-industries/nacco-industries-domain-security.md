---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nacco.com
  spf: true
hosts:
- cert_expires: Aug 30 19:25:05 2026 GMT
  host: www.nacco.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.nacco.com
  https: false
- host: api.nacco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nacco Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NACCO Industries, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NACCO Industries
provider_slug: nacco-industries
slug: nacco-industries-domain-security
source_filename: nacco-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nacco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:25:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.nacco.com\n  https: false\n- host: api.nacco.com\n  https: false\ndomains:\n- domain: nacco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacco-industries/refs/heads/main/security/nacco-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mining
- Housewares
- Industrial
---
