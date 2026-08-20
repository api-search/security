---
api_specs:
- filename: poggio-labs-goalkeeper-openapi.json
  format: json
  label: Goalkeeper API
  slug: goalkeeper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poggio-labs/refs/heads/main/openapi/poggio-labs-goalkeeper-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: poggio.io
  spf: true
hosts:
- cert_expires: Sep 21 18:17:39 2026 GMT
  host: poggio.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:08:51 2026 GMT
  host: api.poggio.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 17:56:34 2026 GMT
  host: mcp.poggio.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poggio Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poggio Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Poggio Labs
provider_slug: poggio-labs
slug: poggio-labs-domain-security
source_filename: poggio-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poggio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.poggio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:08:51 2026 GMT\n  hsts: null\n- host: mcp.poggio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:56:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: poggio.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poggio-labs/refs/heads/main/security/poggio-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Revenue Intelligence
- Sales
- Account Intelligence
- CRM
- Salesforce
- MCP
- AI Agents
- Enterprise
- Open-Source
- Goals
- Gong
- Slack
---
