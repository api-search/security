---
api_specs:
- filename: developer-controlled-wallets.yaml
  format: yaml
  label: Developer-Controlled Wallets
  slug: developer-controlled-wallets
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/developer-controlled-wallets.yaml
- filename: user-controlled-wallets.yaml
  format: yaml
  label: User-Controlled Wallets
  slug: user-controlled-wallets
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/user-controlled-wallets.yaml
- filename: cctp.yaml
  format: yaml
  label: Cross-Chain Transfer Protocol (CCTP)
  slug: cctp
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/cctp.yaml
- filename: gateway.yaml
  format: yaml
  label: Circle Gateway
  slug: gateway
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/gateway.yaml
- filename: smart-contract-platform.yaml
  format: yaml
  label: Smart Contract Platform
  slug: smart-contract-platform
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/smart-contract-platform.yaml
- filename: cpn-ofi.yaml
  format: yaml
  label: Circle Payments Network (CPN)
  slug: cpn
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/cpn-ofi.yaml
- filename: compliance.yaml
  format: yaml
  label: Compliance Engine
  slug: compliance-engine
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/compliance.yaml
- filename: stablefx.yaml
  format: yaml
  label: StableFX
  slug: stablefx
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/stablefx.yaml
- filename: xreserve.yaml
  format: yaml
  label: xReserve
  slug: xreserve
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/xreserve.yaml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:webmaster@circle.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: circle.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.circle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:54:56 2026 GMT
  host: developers.circle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.circle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Circle
provider_slug: circle
slug: circle-domain-security
source_filename: circle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.circle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\n- host: developers.circle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.circle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: circle.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:webmaster@circle.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/security/circle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Compliance
- Cross-Chain
- Currency
- Money
- Payments
- Stablecoin
- Transfers
- USDC
- Wallets
---
