---
api_specs:
- filename: atomtickets-partner-api-openapi.yml
  format: yaml
  label: Atomtickets Partner API
  slug: atomtickets-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomtickets/refs/heads/main/openapi/atomtickets-partner-api-openapi.yml
- filename: atomtickets-partner-api-openapi.yml
  format: yaml
  label: Atomtickets Partner API
  slug: atomtickets-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomtickets/refs/heads/main/openapi/atomtickets-partner-api-openapi.yml
- filename: atomtickets-ping-api-openapi.yml
  format: yaml
  label: Atomtickets Ping API
  slug: atomtickets-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomtickets/refs/heads/main/openapi/atomtickets-ping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atomtickets.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.atomtickets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atomtickets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomtickets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atomtickets
provider_slug: atomtickets
slug: atomtickets-domain-security
source_filename: atomtickets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atomtickets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atomtickets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomtickets/refs/heads/main/security/atomtickets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ticketing
- Event
- Payments
---
