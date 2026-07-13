---
api_specs:
- filename: openapi.json
  format: json
  label: Aha.io REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://www.aha.io/openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aha.io
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.aha.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aha.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aha.io
provider_slug: aha
slug: aha-domain-security
source_filename: aha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aha.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aha.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aha/refs/heads/main/security/aha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Management
- Roadmapping
- Idea Management
- Product Development
- Requirements
- Agile
---
