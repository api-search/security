---
api_specs:
- filename: allspice-io-repos-api-openapi.yml
  format: yaml
  label: AllSpice.io Repos API
  slug: allspice-io-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allspice-io/refs/heads/main/openapi/allspice-io-repos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allspice.io
  spf: true
hosts:
- cert_expires: Dec 19 02:20:12 2026 GMT
  host: allspice.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allspice Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AllSpice.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AllSpice.io
provider_slug: allspice-io
slug: allspice-io-domain-security
source_filename: allspice-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allspice.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 02:20:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allspice.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allspice-io/refs/heads/main/security/allspice-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Collaboration
- Artificial Intelligence
- Design
---
