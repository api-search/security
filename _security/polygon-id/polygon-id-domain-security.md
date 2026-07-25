---
api_specs:
- filename: polygon-id-agent-api-openapi.yml
  format: yaml
  label: Polygon ID Agent API
  slug: polygon-id-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-agent-api-openapi.yml
- filename: polygon-id-auth-api-openapi.yml
  format: yaml
  label: Polygon ID Auth API
  slug: polygon-id-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-auth-api-openapi.yml
- filename: polygon-id-config-api-openapi.yml
  format: yaml
  label: Polygon ID Config API
  slug: polygon-id-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-config-api-openapi.yml
- filename: polygon-id-connection-api-openapi.yml
  format: yaml
  label: Polygon ID Connection API
  slug: polygon-id-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-connection-api-openapi.yml
- filename: polygon-id-credentials-api-openapi.yml
  format: yaml
  label: Polygon ID Credentials API
  slug: polygon-id-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-credentials-api-openapi.yml
- filename: polygon-id-display-methods-api-openapi.yml
  format: yaml
  label: Polygon ID Display Methods API
  slug: polygon-id-display-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-display-methods-api-openapi.yml
- filename: polygon-id-identity-api-openapi.yml
  format: yaml
  label: Polygon ID Identity API
  slug: polygon-id-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-identity-api-openapi.yml
- filename: polygon-id-internal-api-openapi.yml
  format: yaml
  label: Polygon ID Internal API
  slug: polygon-id-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-internal-api-openapi.yml
- filename: polygon-id-key-management-api-openapi.yml
  format: yaml
  label: Polygon ID Key Management API
  slug: polygon-id-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-key-management-api-openapi.yml
- filename: polygon-id-links-api-openapi.yml
  format: yaml
  label: Polygon ID Links API
  slug: polygon-id-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-links-api-openapi.yml
- filename: polygon-id-payment-api-openapi.yml
  format: yaml
  label: Polygon ID Payment API
  slug: polygon-id-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-payment-api-openapi.yml
- filename: polygon-id-public-api-openapi.yml
  format: yaml
  label: Polygon ID Public API
  slug: polygon-id-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-public-api-openapi.yml
- filename: polygon-id-qr-store-api-openapi.yml
  format: yaml
  label: Polygon ID QR Store API
  slug: polygon-id-qr-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-qr-store-api-openapi.yml
- filename: polygon-id-schemas-api-openapi.yml
  format: yaml
  label: Polygon ID Schemas API
  slug: polygon-id-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-schemas-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: privado.id
  spf: true
hosts:
- cert_expires: Sep 11 05:24:25 2026 GMT
  host: www.privado.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:36:59 2026 GMT
  host: docs.privado.id
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:36:59 2026 GMT
  host: issuer-node-core-api-testing.privado.id
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polygon Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polygon ID, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Polygon ID
provider_slug: polygon-id
slug: polygon-id-domain-security
source_filename: polygon-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.privado.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.privado.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:36:59 2026 GMT\n  hsts: false\n- host: issuer-node-core-api-testing.privado.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:36:59 2026 GMT\n  hsts: null\ndomains:\n- domain: privado.id\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/security/polygon-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity
- Verifiable Credentials
- Zero-Knowledge Proofs
- Self-Sovereign Identity
- Decentralized Identity
- Blockchain
- Web3
- KYC
---
