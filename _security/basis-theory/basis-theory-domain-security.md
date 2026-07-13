---
api_specs:
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Tokens API
  slug: basis-theory-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Tokenize / Detokenize API
  slug: basis-theory-tokenize-detokenize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Applications API
  slug: basis-theory-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Proxy API
  slug: basis-theory-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Reactors API
  slug: basis-theory-reactors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory 3D Secure API
  slug: basis-theory-3ds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Tenants API
  slug: basis-theory-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Webhooks API
  slug: basis-theory-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: basistheory.com
  spf: true
hosts:
- cert_expires: Aug 16 06:00:38 2026 GMT
  host: basistheory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 13:39:29 2026 GMT
  host: developers.basistheory.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 01:08:58 2026 GMT
  host: api.basistheory.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basis Theory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basis Theory, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Basis Theory
provider_slug: basis-theory
slug: basis-theory-domain-security
source_filename: basis-theory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basistheory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:00:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.basistheory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 13:39:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.basistheory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:08:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: basistheory.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/security/basis-theory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tokenization
- Data Vault
- PCI Compliance
- Payments
- Security
---
