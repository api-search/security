---
api_specs:
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Tracking Requests API
  slug: tracking-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Shipments API
  slug: shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Containers API
  slug: containers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Transport Events API
  slug: transport-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Terminals & Shipping Lines API
  slug: terminals-shipping-lines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: terminal49.com
  spf: true
hosts:
- cert_expires: Aug 24 10:09:56 2026 GMT
  host: www.terminal49.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 16:01:10 2026 GMT
  host: terminal49.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:36:30 2026 GMT
  host: api.terminal49.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terminal49 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terminal49, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Terminal49
provider_slug: terminal49
slug: terminal49-domain-security
source_filename: terminal49-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terminal49.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:09:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: terminal49.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:01:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.terminal49.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:36:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: terminal49.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/security/terminal49-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Container Tracking
- Ocean Freight
- Supply Chain
- Logistics
- Shipping
---
