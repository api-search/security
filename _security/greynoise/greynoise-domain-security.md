---
api_specs:
- filename: greynoise-openapi.yml
  format: yaml
  label: GreyNoise API
  slug: greynoise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greynoise.io
  spf: true
hosts:
- cert_expires: Aug 28 04:49:56 2026 GMT
  host: www.greynoise.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 08:46:13 2026 GMT
  host: docs.greynoise.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.greynoise.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Greynoise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GreyNoise Intelligence, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GreyNoise Intelligence
provider_slug: greynoise
slug: greynoise-domain-security
source_filename: greynoise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greynoise.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 04:49:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.greynoise.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:46:13 2026 GMT\n  hsts: null\n- host: api.greynoise.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: greynoise.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/security/greynoise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Threat Intelligence
- Cybersecurity
- IP Reputation
- Vulnerability Management
- Network Telemetry
- SOC Automation
- Public APIs
---
