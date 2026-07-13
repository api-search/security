---
api_specs:
- filename: genome-openapi.yml
  format: yaml
  label: Genome
  slug: genome
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/openapi/genome-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: genome.eu
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: genome.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: api.genome.eu
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Genome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genome, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Genome
provider_slug: genome
slug: genome-domain-security
source_filename: genome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genome.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.genome.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: genome.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/security/genome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Payments
---
