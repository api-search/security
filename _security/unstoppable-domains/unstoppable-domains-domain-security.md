---
api_specs:
- filename: unstoppable-domains-resolution-api-openapi.yaml
  format: yaml
  label: Unstoppable Domains Resolution API
  slug: unstoppable-domains-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-resolution-api-openapi.yaml
- filename: unstoppable-domains-partner-api-openapi.yaml
  format: yaml
  label: Unstoppable Domains Partner API
  slug: unstoppable-domains-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-partner-api-openapi.yaml
- filename: unstoppable-domains-reseller-api-openapi.yaml
  format: yaml
  label: Unstoppable Domains Reseller API
  slug: unstoppable-domains-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-reseller-api-openapi.yaml
- filename: unstoppable-domains-user-api-openapi.json
  format: json
  label: Unstoppable Domains User API
  slug: unstoppable-domains-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/openapi/unstoppable-domains-user-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unstoppabledomains.com
  spf: true
hosts:
- cert_expires: Sep  7 18:39:55 2026 GMT
  host: unstoppabledomains.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 17:17:01 2026 GMT
  host: docs.unstoppabledomains.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 18:39:55 2026 GMT
  host: api.unstoppabledomains.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unstoppable Domains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unstoppable Domains, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Unstoppable Domains
provider_slug: unstoppable-domains
slug: unstoppable-domains-domain-security
source_filename: unstoppable-domains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unstoppabledomains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:39:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unstoppabledomains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:17:01 2026 GMT\n  hsts: false\n- host: api.unstoppabledomains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:39:55 2026 GMT\n  hsts: null\ndomains:\n- domain: unstoppabledomains.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstoppable-domains/refs/heads/main/security/unstoppable-domains-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- Domain Names
- NFT Domains
- Crypto
- Resolution
- DNS
- Decentralized
- Ethereum
- Polygon
---
