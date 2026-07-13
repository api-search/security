---
api_specs:
- filename: chronosphere-openapi.yml
  format: yaml
  label: Chronosphere
  slug: chronosphere
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronosphere/refs/heads/main/openapi/chronosphere-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chronosphere.io
  spf: true
hosts:
- cert_expires: Sep 26 07:13:04 2026 GMT
  host: chronosphere.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chronosphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronosphere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chronosphere
provider_slug: chronosphere
slug: chronosphere-domain-security
source_filename: chronosphere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chronosphere.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:13:04 2026 GMT\n  hsts: false\ndomains:\n- domain: chronosphere.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronosphere/refs/heads/main/security/chronosphere-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AIOps
- Observability
---
