---
api_specs:
- filename: cobli-public-api-openapi.yml
  format: yaml
  label: Cobli Public API
  slug: cobli-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobli/refs/heads/main/openapi/cobli-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cobli.co
  spf: true
hosts:
- cert_expires: Dec 10 20:04:03 2026 GMT
  host: www.cobli.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cobli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cobli
provider_slug: cobli
slug: cobli-domain-security
source_filename: cobli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cobli.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:04:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cobli.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobli/refs/heads/main/security/cobli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
