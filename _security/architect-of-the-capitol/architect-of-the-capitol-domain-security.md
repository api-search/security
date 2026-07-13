---
api_specs:
- filename: aoc-data-api.yaml
  format: yaml
  label: Architect of the Capitol Data API
  slug: aoc-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/openapi/aoc-data-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aoc.gov
  spf: true
hosts:
- cert_expires: Aug 28 11:28:56 2026 GMT
  host: www.aoc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.aoc.gov
  https: false
kind: domain-security
layout: security
method: probed
name: Architect Of The Capitol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Architect of the Capitol, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
slug: architect-of-the-capitol-domain-security
source_filename: architect-of-the-capitol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aoc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:28:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aoc.gov\n  https: false\ndomains:\n- domain: aoc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/security/architect-of-the-capitol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
---
