---
api_specs:
- filename: hiveagentiq-com-hivetrust-openapi.json
  format: json
  label: HiveTrust KYA Identity & Trust API
  slug: hivetrust-kya-identity-trust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivetrust-openapi.json
- filename: hiveagentiq-com-hivegate-openapi.json
  format: json
  label: HiveGate Admission, Identity & Pricing Tier API
  slug: hivegate-admission-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivegate-openapi.json
- filename: hiveagentiq-com-hivebank-openapi.json
  format: json
  label: HiveBank Treasury Attestation & Settlement API
  slug: hivebank-treasury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivebank-openapi.json
- filename: hiveagentiq-com-hivelaw-openapi.json
  format: json
  label: HiveLaw AI Legal Contracts & Compliance API
  slug: hivelaw-legal-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivelaw-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hiveagentiq.com
  spf: true
- caa:
  - 0 iodef "mailto:security+caafailure@render.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onrender.com
  spf: false
hosts:
- cert_expires: Oct 29 07:50:07 2026 GMT
  host: hiveagentiq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 21:54:17 2026 GMT
  host: hivebank.onrender.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 12:46:32 2026 GMT
  host: hivegate.hiveagentiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Hiveagentiq Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hive Agent IQ, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hive Agent IQ
provider_slug: hiveagentiq-com
slug: hiveagentiq-com-domain-security
source_filename: hiveagentiq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiveagentiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 07:50:07 2026 GMT\n  hsts: null\n- host: hivebank.onrender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 21:54:17 2026 GMT\n  hsts: null\n- host: hivegate.hiveagentiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 12:46:32 2026 GMT\n  hsts: false\ndomains:\n- domain: hiveagentiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: onrender.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security+caafailure@render.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/security/hiveagentiq-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Decentralized Identity
- Verifiable Credentials
- Trust Scoring
- Stablecoins
- Insurance
- Compliance
- Agent-Native
- United States
---
