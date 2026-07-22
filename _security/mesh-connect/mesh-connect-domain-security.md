---
api_specs:
- filename: mesh-connect-openapi-original.json
  format: json
  label: Mesh Connect Integration API
  slug: mesh-connect-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-openapi-original.json
- filename: mesh-connect-admin-openapi-original.json
  format: json
  label: Mesh Admin API
  slug: mesh-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-admin-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meshconnect.com
  spf: true
hosts:
- cert_expires: Oct 15 02:09:24 2026 GMT
  host: www.meshconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: admin-api.meshconnect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:30:57 2026 GMT
  host: integration-api.meshconnect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mesh Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mesh Connect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mesh Connect
provider_slug: mesh-connect
slug: mesh-connect-domain-security
source_filename: mesh-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:09:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: admin-api.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: integration-api.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:30:57 2026 GMT\n  hsts: null\ndomains:\n- domain: meshconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/security/mesh-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Infrastructure
- Crypto Payments
- Digital Assets
- Wallets
- Exchanges
- Embedded Finance
- Stablecoins
- Payments
---
