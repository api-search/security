---
api_specs:
- filename: phoslabs-io-openapi.yml
  format: yaml
  label: Behavioral Science API
  slug: behavioral-science-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-openapi.yml
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
