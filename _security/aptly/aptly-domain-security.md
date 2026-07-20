---
api_specs:
- filename: aptly-openapi-original.yml
  format: yaml
  label: Aptly Core API
  slug: aptly-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getaptly.com
  spf: true
hosts:
- cert_expires: Sep 18 22:42:28 2026 GMT
  host: getaptly.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 23:03:31 2026 GMT
  host: core-api.getaptly.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aptly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aptly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aptly
provider_slug: aptly
slug: aptly-domain-security
source_filename: aptly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getaptly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:42:28 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: core-api.getaptly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:03:31 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: getaptly.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/security/aptly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud Saas
- Property Management
- Real Estate
- PropTech
- CRM
- Workflow Automation
- AI Agents
- Communications
- MCP
---
