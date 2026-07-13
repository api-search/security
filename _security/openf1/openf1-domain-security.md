---
api_specs:
- filename: openf1-openapi.yml
  format: yaml
  label: OpenF1 API
  slug: openf1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openf1/refs/heads/main/openapi/openf1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openf1.org
  spf: true
hosts:
- cert_expires: Sep 22 23:04:22 2026 GMT
  host: openf1.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:06:58 2026 GMT
  host: api.openf1.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openf1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenF1, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OpenF1
provider_slug: openf1
slug: openf1-domain-security
source_filename: openf1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openf1.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:04:22 2026 GMT\n  hsts: false\n- host: api.openf1.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:06:58 2026 GMT\n  hsts: null\ndomains:\n- domain: openf1.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openf1/refs/heads/main/security/openf1-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Formula 1
- Motorsport
- Telemetry
- Real-Time
- Sports
---
