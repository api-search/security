---
api_specs:
- filename: tradeshift-external-api-openapi.yml
  format: yaml
  label: Tradeshift External API
  slug: tradeshift-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-external-api-openapi.yml
- filename: tradeshift-mcp-bridge-openapi.yml
  format: yaml
  label: Tradeshift MCP Server
  slug: tradeshift-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-mcp-bridge-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tradeshift.com
  spf: true
hosts:
- cert_expires: Oct 26 22:30:36 2026 GMT
  host: tradeshift.com
  hsts: true
  hsts_max_age: 31536001
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:43:14 2026 GMT
  host: developers.tradeshift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 05:37:34 2026 GMT
  host: api.tradeshift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradeshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradeshift, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tradeshift
provider_slug: tradeshift
slug: tradeshift-domain-security
source_filename: tradeshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 22:30:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536001\n- host: developers.tradeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tradeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 05:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tradeshift.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/security/tradeshift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- e-invoicing
- accounts-payable
- ap-automation
- procure-to-pay
- supply-chain
- b2b-commerce
- invoicing
- ubl
- peppol
- e-invoicing-compliance
- supplier-network
- business-documents
- fintech
- mcp
- agent-native
---
