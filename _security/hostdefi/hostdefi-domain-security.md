---
api_specs:
- filename: hostdefi-token-risk-api-openapi.yml
  format: yaml
  label: HostDeFi Token Risk API
  slug: hostdefi-token-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-token-risk-api-openapi.yml
- filename: hostdefi-analyze-token-api-openapi.yml
  format: yaml
  label: HostDeFi Analyze Token API
  slug: hostdefi-analyze-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-analyze-token-api-openapi.yml
- filename: hostdefi-health-api-openapi.yml
  format: yaml
  label: HostDeFi Health API
  slug: hostdefi-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-health-api-openapi.yml
- filename: hostdefi-keys-api-openapi.yml
  format: yaml
  label: HostDeFi Keys API
  slug: hostdefi-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-keys-api-openapi.yml
- filename: hostdefi-scan-api-openapi.yml
  format: yaml
  label: HostDeFi Scan API
  slug: hostdefi-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-scan-api-openapi.yml
- filename: hostdefi-usage-api-openapi.yml
  format: yaml
  label: HostDeFi Usage API
  slug: hostdefi-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-usage-api-openapi.yml
- filename: hostdefi-x402-machine-payable-api-openapi.yml
  format: yaml
  label: HostDeFi x402 (machine-payable) API
  slug: hostdefi-x402-machine-payable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostdefi/openapi/hostdefi-x402-machine-payable-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hostdefi.com
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: railway.app
  spf: true
hosts:
- cert_expires: Jan 14 20:56:51 2027 GMT
  host: hostdefi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 03:01:42 2026 GMT
  host: awake-integrity-production-faa0.up.railway.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: HostDeFi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HostDeFi, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HostDeFi
provider_slug: hostdefi
slug: hostdefi-domain-security
source_filename: hostdefi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostdefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:56:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: awake-integrity-production-faa0.up.railway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:01:42 2026 GMT\n  hsts: null\ndomains:\n- domain: hostdefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: railway.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hostdefi/security/hostdefi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Solana
- Token Risk
- DeFi
- rug-pull
- x402
- A2A
---
