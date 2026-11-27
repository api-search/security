---
api_specs:
- filename: markaestro-com-openapi-generated.yml
  format: yaml
  label: Markaestro API
  slug: markaestro-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markaestro-com/openapi/_ae-authored/markaestro-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: markaestro.com
  spf: true
hosts:
- cert_expires: Feb 13 07:01:15 2027 GMT
  host: markaestro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Markaestro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markaestro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Markaestro
provider_slug: markaestro-com
slug: markaestro-com-domain-security
source_filename: markaestro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markaestro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 07:01:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: markaestro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/markaestro-com/security/markaestro-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media Scheduling
- AI Agents
- Evergreen Recycling
- Client Approval
- Calendar
---
