---
api_specs:
- filename: neighbor-openapi.yml
  format: yaml
  label: Neighbor
  slug: neighbor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbor/refs/heads/main/openapi/neighbor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neighbor.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.neighbor.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Neighbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neighbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Neighbor
provider_slug: neighbor
slug: neighbor-domain-security
source_filename: neighbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.neighbor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: neighbor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neighbor/refs/heads/main/security/neighbor-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Storage
- Marketplace
- Reporting
---
