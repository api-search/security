---
api_specs:
- filename: simba-chain-member-service-openapi.json
  format: json
  label: SIMBA Blocks Member Service API
  slug: simba-chain-member-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/openapi/simba-chain-member-service-openapi.json
- filename: simba-chain-member-service-validator-openapi.json
  format: json
  label: SIMBA Blocks Authentication Service API
  slug: simba-chain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/openapi/simba-chain-member-service-validator-openapi.json
description: ''
domains:
- caa:
  - 0 issue "buypass.com"
  - 0 issue "buypass.no"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simbachain.com
  spf: true
hosts:
- cert_expires: Nov  9 20:27:36 2026 GMT
  host: simbachain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 22:39:09 2026 GMT
  host: docs.simbachain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: blocks.simbachain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simba Chain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SIMBA Chain, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SIMBA Chain
provider_slug: simba-chain
slug: simba-chain-domain-security
source_filename: simba-chain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simbachain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 20:27:36 2026 GMT\n  hsts: false\n- host: docs.simbachain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 22:39:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blocks.simbachain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: simbachain.com\n  dnssec: false\n  caa:\n  - 0 issue \"buypass.com\"\n  - 0 issue \"buypass.no\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/security/simba-chain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Supply Chain
- Traceability
- Digital Product Passport
- Smart Contracts
- Identity
- Verifiable Credentials
- Defense
- Government
- Data Management
---
