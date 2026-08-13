---
api_specs:
- filename: elixir-medical-wordpress-content-openapi.yml
  format: yaml
  label: Elixir Medical Website Content API (WordPress REST)
  slug: elixir-medical-wordpress-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/openapi/elixir-medical-wordpress-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elixirmedical.com
  spf: true
hosts:
- cert_expires: Oct 20 20:48:10 2026 GMT
  host: elixirmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elixir Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elixir Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elixir Medical
provider_slug: elixir-medical
slug: elixir-medical-domain-security
source_filename: elixir-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elixirmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 20:48:10 2026 GMT\n  hsts: false\ndomains:\n- domain: elixirmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elixir-medical/refs/heads/main/security/elixir-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Health
- Cardiovascular
- Coronary Intervention
- Implants
- Life Sciences
- Content
- WordPress
---
