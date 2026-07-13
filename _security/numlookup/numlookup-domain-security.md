---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: numlookupapi.com
  spf: true
hosts:
- cert_expires: Oct  7 06:44:54 2026 GMT
  host: numlookupapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numlookup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numlookup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Numlookup
provider_slug: numlookup
slug: numlookup-domain-security
source_filename: numlookup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numlookupapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 06:44:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numlookupapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numlookup/refs/heads/main/security/numlookup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Phone
- Public APIs
---
