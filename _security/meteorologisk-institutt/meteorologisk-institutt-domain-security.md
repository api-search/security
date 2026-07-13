---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: met.no
  spf: true
hosts:
- cert_expires: Nov  7 06:51:30 2026 GMT
  host: api.met.no
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meteorologisk Institutt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meteorologisk Institutt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Meteorologisk Institutt
provider_slug: meteorologisk-institutt
slug: meteorologisk-institutt-domain-security
source_filename: meteorologisk-institutt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.met.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 06:51:30 2026 GMT\n  hsts: false\ndomains:\n- domain: met.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meteorologisk-institutt/refs/heads/main/security/meteorologisk-institutt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Weather
- Public APIs
---
