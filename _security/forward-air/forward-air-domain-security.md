---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forwardair.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.forwardair.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.forwardair.com
  https: false
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.forwardair.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Forward Air Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forward Air, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forward Air
provider_slug: forward-air
slug: forward-air-domain-security
source_filename: forward-air-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forwardair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: developer.forwardair.com\n  https: false\n- host: api.forwardair.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: forwardair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forward-air/refs/heads/main/security/forward-air-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Freight
- Air Cargo
- Logistics
---
