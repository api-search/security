---
api_specs:
- filename: thumbtack-demand-openapi.yml
  format: yaml
  label: Thumbtack Demand API
  slug: thumbtack-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-demand-openapi.yml
- filename: thumbtack-pro-openapi.yml
  format: yaml
  label: Thumbtack Pro API
  slug: thumbtack-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-pro-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thumbtack.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.thumbtack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: developers.thumbtack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.thumbtack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thumbtack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thumbtack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thumbtack
provider_slug: thumbtack
slug: thumbtack-domain-security
source_filename: thumbtack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thumbtack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: developers.thumbtack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.thumbtack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thumbtack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/security/thumbtack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Local Services
- Marketplace
- Home Services
- Leads
- Partner API
---
