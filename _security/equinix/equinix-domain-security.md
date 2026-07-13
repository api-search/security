---
api_specs:
- filename: fabric-openapi-original.yml
  format: yaml
  label: Equinix Fabric API
  slug: fabric
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/fabric-openapi-original.yml
- filename: metal-openapi-original.yml
  format: yaml
  label: Equinix Metal API
  slug: metal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/metal-openapi-original.yml
- filename: eia-openapi-original.yml
  format: yaml
  label: Equinix Internet Access API
  slug: internet-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/eia-openapi-original.yml
- filename: lookup-openapi-original.yml
  format: yaml
  label: Equinix Lookup API
  slug: lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/lookup-openapi-original.yml
- filename: orders-openapi-original.yml
  format: yaml
  label: Equinix Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/orders-openapi-original.yml
- filename: orderhistory-openapi-original.yml
  format: yaml
  label: Equinix Order History API
  slug: order-history
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/orderhistory-openapi-original.yml
- filename: securecabinet-openapi-original.yml
  format: yaml
  label: Equinix Secure Cabinet API
  slug: secure-cabinet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/securecabinet-openapi-original.yml
- filename: smarthands-openapi-original.yml
  format: yaml
  label: Equinix Smart Hands API
  slug: smart-hands
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/smarthands-openapi-original.yml
- filename: accesstoken-openapi-original.yml
  format: yaml
  label: Equinix API Authentication
  slug: access-token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/accesstoken-openapi-original.yml
- filename: sts-openapi-original.yml
  format: yaml
  label: Equinix Security Token Service
  slug: sts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/sts-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equinix.com
  spf: true
hosts:
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: www.equinix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: developer.equinix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.equinix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equinix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equinix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Equinix
provider_slug: equinix
slug: equinix-domain-security
source_filename: equinix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.equinix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.equinix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: null\n- host: api.equinix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: equinix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/security/equinix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
- Data Centers
- Interconnection
- Colocation
- Bare Metal
- Cloud Infrastructure
- Networking
---
