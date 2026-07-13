---
api_specs:
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Menu Sync API
  slug: menu-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chowly.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chowlyinc.com
  spf: true
hosts:
- cert_expires: Aug 24 00:16:04 2026 GMT
  host: www.chowly.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 00:54:14 2026 GMT
  host: api.chowlyinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: partners.olo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chowly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chowly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chowly
provider_slug: chowly
slug: chowly-domain-security
source_filename: chowly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chowly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:16:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.chowlyinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:54:14 2026 GMT\n  hsts: false\n- host: partners.olo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chowly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: chowlyinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/security/chowly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Online Ordering
- Delivery
- POS Integration
- Menu Sync
---
