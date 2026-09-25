---
api_specs:
- filename: optionsahoy-com-openapi.json
  format: json
  label: OptionsAhoy Calculator API
  slug: optionsahoy-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optionsahoy-com/refs/heads/main/openapi/optionsahoy-com-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: optionsahoy.com
  spf: true
hosts:
- cert_expires: Nov 19 10:25:18 2026 GMT
  host: optionsahoy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Optionsahoy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OptionsAhoy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OptionsAhoy
provider_slug: optionsahoy-com
slug: optionsahoy-com-domain-security
source_filename: optionsahoy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optionsahoy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 10:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: optionsahoy.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optionsahoy-com/refs/heads/main/security/optionsahoy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Equity Compensation
- Tax
- Stock Options
- Financial Planning
- Personal Finance
- Fintech
- Calculators
- MCP
- A2A
- Agent-Native
- Deterministic
- United States
---
