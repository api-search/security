---
api_specs:
- filename: polysign-abc-accounts-api-openapi.yml
  format: yaml
  label: PolySign ABC Accounts API
  slug: polysign-abc-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-accounts-api-openapi.yml
- filename: polysign-abc-memorials-api-openapi.yml
  format: yaml
  label: PolySign ABC Memorials API
  slug: polysign-abc-memorials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-memorials-api-openapi.yml
- filename: polysign-abc-signing-api-openapi.yml
  format: yaml
  label: PolySign ABC Signing API
  slug: polysign-abc-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-signing-api-openapi.yml
- filename: polysign-abc-testnet-api-openapi.yml
  format: yaml
  label: PolySign ABC Testnet API
  slug: polysign-abc-testnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-testnet-api-openapi.yml
- filename: polysign-asset-api-openapi.yml
  format: yaml
  label: PolySign Asset API
  slug: polysign-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-asset-api-openapi.yml
- filename: polysign-authentication-api-openapi.yml
  format: yaml
  label: PolySign Authentication API
  slug: polysign-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-authentication-api-openapi.yml
- filename: polysign-beneficiary-authorization-api-openapi.yml
  format: yaml
  label: PolySign beneficiary authorization API
  slug: polysign-beneficiary-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-beneficiary-authorization-api-openapi.yml
- filename: polysign-book-transfer-api-openapi.yml
  format: yaml
  label: PolySign book transfer API
  slug: polysign-book-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-book-transfer-api-openapi.yml
- filename: polysign-book-transfer-confirmation-api-openapi.yml
  format: yaml
  label: PolySign book transfer confirmation API
  slug: polysign-book-transfer-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-book-transfer-confirmation-api-openapi.yml
- filename: polysign-escrow-authorization-api-openapi.yml
  format: yaml
  label: PolySign escrow authorization API
  slug: polysign-escrow-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-escrow-authorization-api-openapi.yml
- filename: polysign-investor-api-openapi.yml
  format: yaml
  label: PolySign Investor API
  slug: polysign-investor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-investor-api-openapi.yml
- filename: polysign-order-api-openapi.yml
  format: yaml
  label: PolySign Order API
  slug: polysign-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-order-api-openapi.yml
- filename: polysign-partner-api-openapi.yml
  format: yaml
  label: PolySign Partner API
  slug: polysign-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-partner-api-openapi.yml
- filename: polysign-settlement-api-openapi.yml
  format: yaml
  label: PolySign Settlement API
  slug: polysign-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-settlement-api-openapi.yml
- filename: polysign-settlement-confirmation-api-openapi.yml
  format: yaml
  label: PolySign settlement confirmation API
  slug: polysign-settlement-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-settlement-confirmation-api-openapi.yml
- filename: polysign-system-api-openapi.yml
  format: yaml
  label: PolySign System API
  slug: polysign-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-system-api-openapi.yml
- filename: polysign-utility-api-openapi.yml
  format: yaml
  label: PolySign Utility API
  slug: polysign-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polysign.io
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.polysign.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: docs.polynet.sandbox.polysign.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polysign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolySign, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PolySign
provider_slug: polysign
slug: polysign-domain-security
source_filename: polysign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polysign.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: docs.polynet.sandbox.polysign.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: polysign.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/security/polysign-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- digital-assets
- blockchain
- institutional-custody
- settlement
- escrow
- capital-markets
- payments
- fintech
- distributed-ledger
- atomicnet
---
