---
api_specs:
- filename: nord-security-nordstellar-enterprise-data-api-openapi.json
  format: json
  label: NordStellar Enterprise Data API
  slug: nordstellar-enterprise-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-enterprise-data-api-openapi.json
- filename: nord-security-nordstellar-company-risk-scoring-api-openapi.json
  format: json
  label: NordStellar Company Risk Scoring API
  slug: nordstellar-company-risk-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json
- filename: nord-security-nordstellar-cybersec-api-openapi.json
  format: json
  label: NordStellar Cybersec API
  slug: nordstellar-cybersec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-cybersec-api-openapi.json
- filename: nord-security-nordstellar-partners-api-openapi.json
  format: json
  label: NordStellar Partners API
  slug: nordstellar-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-partners-api-openapi.json
- filename: nord-security-nordstellar-platform-integration-api-v3-openapi.json
  format: json
  label: NordStellar Platform Integrations API
  slug: nordstellar-platform-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-platform-integration-api-v3-openapi.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nordsecurity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nordstellar.com
  spf: true
hosts:
- cert_expires: Sep 23 02:20:09 2026 GMT
  host: nordsecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:47:04 2026 GMT
  host: docs.nordstellar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:47:04 2026 GMT
  host: enterprise-data-api.nordstellar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nord Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nord Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nord Security
provider_slug: nord-security
slug: nord-security-domain-security
source_filename: nord-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nordsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nordstellar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:47:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: enterprise-data-api.nordstellar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:47:04 2026 GMT\n  hsts: null\ndomains:\n- domain: nordsecurity.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nordstellar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/security/nord-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Threat Intelligence
- Dark Web Monitoring
- Attack Surface Management
- Breach Intelligence
- VPN
- Password Management
- Network Security
- Zero Trust
- Privacy
- MCP
- Agent Skills
- gRPC
- Company
---
