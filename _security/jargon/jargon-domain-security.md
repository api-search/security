---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jargon.sh
  spf: false
hosts:
- cert_expires: Aug 24 13:01:52 2026 GMT
  host: jargon.sh
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jargon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jargon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Jargon
provider_slug: jargon
slug: jargon-domain-security
source_filename: jargon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jargon.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: jargon.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jargon/refs/heads/main/security/jargon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- Data Modelling
- Domain Driven Design
- Domains
- JSON Schema
- OpenAPI
- Platform
---
