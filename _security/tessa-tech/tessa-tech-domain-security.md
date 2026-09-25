---
api_specs:
- filename: tessa-tech-agent-directory-openapi.yml
  format: yaml
  label: TESSA Agent Directory API
  slug: tessa-agent-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessa-tech/refs/heads/main/openapi/tessa-tech-agent-directory-openapi.yml
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
  domain: tessa.tech
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: complianceregistry.net
  spf: false
hosts:
- cert_expires: Nov  5 09:44:52 2026 GMT
  host: tessa.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 17:51:54 2026 GMT
  host: aiagent.tessa.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 18:22:48 2026 GMT
  host: complianceregistry.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Tessa Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TESSA Marketing & Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TESSA Marketing & Technology
provider_slug: tessa-tech
slug: tessa-tech-domain-security
source_filename: tessa-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tessa.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 09:44:52 2026 GMT\n  hsts: false\n- host: aiagent.tessa.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 17:51:54 2026 GMT\n  hsts: null\n- host: complianceregistry.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 18:22:48 2026 GMT\n  hsts: null\ndomains:\n- domain: tessa.tech\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: complianceregistry.net\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessa-tech/refs/heads/main/security/tessa-tech-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Digital Marketing
- SEO
- Web Development
- Accessibility
- AI Agent Readiness
- Professional Services
- Agent Directory
- A2A
- MCP
- Agent-Native
- Company
---
