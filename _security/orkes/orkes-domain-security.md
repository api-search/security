---
api_specs:
- filename: orkes-conductor-api.yml
  format: yaml
  label: Orkes
  slug: orkes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-conductor-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orkes.io
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: orkes.io
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orkes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orkes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orkes
provider_slug: orkes
slug: orkes-domain-security
source_filename: orkes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orkes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1800\ndomains:\n- domain: orkes.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/security/orkes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microservices
---
