---
api_specs:
- filename: hostdefi-token-risk-api-openapi.yml
  format: yaml
  label: HostDeFi Token Risk API
  slug: hostdefi-token-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-token-risk-api-openapi.yml
- filename: hostdefi-analyze-token-api-openapi.yml
  format: yaml
  label: HostDeFi Analyze Token API
  slug: hostdefi-analyze-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-analyze-token-api-openapi.yml
- filename: hostdefi-health-api-openapi.yml
  format: yaml
  label: HostDeFi Health API
  slug: hostdefi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-health-api-openapi.yml
- filename: hostdefi-keys-api-openapi.yml
  format: yaml
  label: HostDeFi Keys API
  slug: hostdefi-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-keys-api-openapi.yml
- filename: hostdefi-scan-api-openapi.yml
  format: yaml
  label: HostDeFi Scan API
  slug: hostdefi-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-scan-api-openapi.yml
- filename: hostdefi-usage-api-openapi.yml
  format: yaml
  label: HostDeFi Usage API
  slug: hostdefi-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-usage-api-openapi.yml
- filename: hostdefi-x402-machine-payable-api-openapi.yml
  format: yaml
  label: HostDeFi x402 (machine-payable) API
  slug: hostdefi-x402-machine-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-x402-machine-payable-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hostdefi.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: railway.app
  spf: true
hosts:
- cert_expires: Nov 16 19:12:49 2026 GMT
  host: hostdefi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 02:40:54 2026 GMT
  host: awake-integrity-production-faa0.up.railway.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hostdefi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HostDeFi, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HostDeFi
provider_slug: hostdefi
slug: hostdefi-domain-security
source_filename: hostdefi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostdefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 19:12:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: awake-integrity-production-faa0.up.railway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:40:54 2026 GMT\n  hsts: false\ndomains:\n- domain: hostdefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: railway.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/security/hostdefi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Solana
- Token Risk
- DeFi
- rug pull
- x402
---
