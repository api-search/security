---
api_specs:
- filename: synthego-order-openapi.json
  format: json
  label: Synthego Order API
  slug: synthego-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthego/refs/heads/main/openapi/synthego-order-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synthego.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.synthego.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Synthego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthego, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synthego
provider_slug: synthego
slug: synthego-domain-security
source_filename: synthego-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.synthego.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: synthego.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthego/refs/heads/main/security/synthego-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Health Tech
- Genomics
- CRISPR
- Biotechnology
- Life Sciences
- Synthetic Biology
- Ordering
---
