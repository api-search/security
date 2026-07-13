---
api_specs:
- filename: godaddy-domains-openapi.json
  format: json
  label: GoDaddy Domains API
  slug: domains
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-domains-openapi.json
- filename: godaddy-certificates-openapi.json
  format: json
  label: GoDaddy Certificates API
  slug: certificates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-certificates-openapi.json
- filename: godaddy-shoppers-openapi.json
  format: json
  label: GoDaddy Shoppers API
  slug: shoppers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-shoppers-openapi.json
- filename: godaddy-subscriptions-openapi.json
  format: json
  label: GoDaddy Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-subscriptions-openapi.json
- filename: godaddy-orders-openapi.json
  format: json
  label: GoDaddy Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-orders-openapi.json
- filename: godaddy-aftermarket-openapi.json
  format: json
  label: GoDaddy Aftermarket API
  slug: aftermarket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-aftermarket-openapi.json
- filename: godaddy-abuse-openapi.json
  format: json
  label: GoDaddy Abuse API
  slug: abuse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-abuse-openapi.json
- filename: godaddy-agreements-openapi.json
  format: json
  label: GoDaddy Agreements API
  slug: agreements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-agreements-openapi.json
- filename: godaddy-countries-openapi.json
  format: json
  label: GoDaddy Countries API
  slug: countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-countries-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: godaddy.com
  spf: true
hosts:
- cert_expires: Nov  2 23:48:17 2026 GMT
  host: www.godaddy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:48:17 2026 GMT
  host: developer.godaddy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:48:17 2026 GMT
  host: api.godaddy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Godaddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoDaddy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoDaddy
provider_slug: godaddy
slug: godaddy-domain-security
source_filename: godaddy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.godaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:48:17 2026 GMT\n  hsts: null\n- host: developer.godaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:48:17 2026 GMT\n  hsts: false\n- host: api.godaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:48:17 2026 GMT\n  hsts: null\ndomains:\n- domain: godaddy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/security/godaddy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aftermarket
- Certificates
- DNS
- Domains
- Hosting
- Registrar
---
