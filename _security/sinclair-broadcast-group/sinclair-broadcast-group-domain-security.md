---
api_specs:
- filename: sinclair-broadcast-group-content-openapi.yml
  format: yaml
  label: Sinclair Corporate Content API
  slug: sinclair-corporate-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/openapi/sinclair-broadcast-group-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sbgi.net
  spf: true
hosts:
- cert_expires: Sep 14 05:59:51 2026 GMT
  host: sbgi.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sinclair Broadcast Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sinclair, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sinclair, Inc.
provider_slug: sinclair-broadcast-group
slug: sinclair-broadcast-group-domain-security
source_filename: sinclair-broadcast-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sbgi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:59:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: sbgi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinclair-broadcast-group/refs/heads/main/security/sinclair-broadcast-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Television
- Local News
- Sports Media
- Regional Sports Networks
- Digital Marketing
- Advertising Technology
- NextGen TV
- ATSC 3.0
- Media
---
