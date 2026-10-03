---
api_specs:
- filename: phoslabs-io-audit-api-openapi.yml
  format: yaml
  label: Phos Labs Audit API
  slug: phoslabs-io-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-audit-api-openapi.yml
- filename: phoslabs-io-copy-api-openapi.yml
  format: yaml
  label: Phos Labs Copy API
  slug: phoslabs-io-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-copy-api-openapi.yml
- filename: phoslabs-io-detect-biases-api-openapi.yml
  format: yaml
  label: Phos Labs Detect Biases API
  slug: phoslabs-io-detect-biases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-detect-biases-api-openapi.yml
- filename: phoslabs-io-diagnose-api-openapi.yml
  format: yaml
  label: Phos Labs Diagnose API
  slug: phoslabs-io-diagnose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-diagnose-api-openapi.yml
- filename: phoslabs-io-fix-checkout-api-openapi.yml
  format: yaml
  label: Phos Labs Fix Checkout API
  slug: phoslabs-io-fix-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-fix-checkout-api-openapi.yml
- filename: phoslabs-io-pricing-api-openapi.yml
  format: yaml
  label: Phos Labs Pricing API
  slug: phoslabs-io-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-pricing-api-openapi.yml
- filename: phoslabs-io-tools-api-openapi.yml
  format: yaml
  label: Phos Labs Tools API
  slug: phoslabs-io-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-tools-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: phoslabs.io
  spf: true
hosts:
- cert_expires: Nov 23 16:15:12 2026 GMT
  host: phoslabs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Phoslabs Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phos Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Phos Labs
provider_slug: phoslabs-io
slug: phoslabs-io-domain-security
source_filename: phoslabs-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phoslabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 16:15:12 2026 GMT\n  hsts: false\ndomains:\n- domain: phoslabs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/security/phoslabs-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Behavioral Science
- Conversion Optimization
- E-Commerce
- Pricing
- Copywriting
- AI Agents
- MCP
- A2A
- Decision Intelligence
- Agentic Commerce
---
