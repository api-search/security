---
api_specs:
- filename: tripgic-openapi-generated.yml
  format: yaml
  label: Tripgic API
  slug: tripgic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripgic/refs/heads/main/openapi/_ae-authored/tripgic-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tripgic.com
  spf: true
hosts:
- cert_expires: Dec 24 05:02:55 2026 GMT
  host: www.tripgic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tripgic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripgic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tripgic
provider_slug: tripgic
slug: tripgic-domain-security
source_filename: tripgic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tripgic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 05:02:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tripgic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripgic/refs/heads/main/security/tripgic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- API
- Booking
- Aggregator
---
