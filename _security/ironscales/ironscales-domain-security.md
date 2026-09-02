---
api_specs:
- filename: ironscales-authorization-api-openapi.yml
  format: yaml
  label: IRONSCALES Authorization API
  slug: ironscales-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-authorization-api-openapi.yml
- filename: ironscales-campaigns-api-openapi.yml
  format: yaml
  label: IRONSCALES Campaigns API
  slug: ironscales-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-campaigns-api-openapi.yml
- filename: ironscales-deepfake-api-openapi.yml
  format: yaml
  label: IRONSCALES Deepfake API
  slug: ironscales-deepfake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-deepfake-api-openapi.yml
- filename: ironscales-emails-api-openapi.yml
  format: yaml
  label: IRONSCALES Emails API
  slug: ironscales-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-emails-api-openapi.yml
- filename: ironscales-incident-api-openapi.yml
  format: yaml
  label: IRONSCALES Incident API
  slug: ironscales-incident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-incident-api-openapi.yml
- filename: ironscales-mailboxes-api-openapi.yml
  format: yaml
  label: IRONSCALES Mailboxes API
  slug: ironscales-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-mailboxes-api-openapi.yml
- filename: ironscales-mitigation-api-openapi.yml
  format: yaml
  label: IRONSCALES Mitigation API
  slug: ironscales-mitigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-mitigation-api-openapi.yml
- filename: ironscales-sat-api-openapi.yml
  format: yaml
  label: IRONSCALES SAT API
  slug: ironscales-sat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-sat-api-openapi.yml
- filename: ironscales-settings-api-openapi.yml
  format: yaml
  label: IRONSCALES Settings API
  slug: ironscales-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ironscales.com
  spf: true
hosts:
- cert_expires: Sep 19 10:36:06 2026 GMT
  host: ironscales.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: appapi.ironscales.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: mcp.ironscales.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ironscales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IRONSCALES, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IRONSCALES
provider_slug: ironscales
slug: ironscales-domain-security
source_filename: ironscales-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ironscales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 10:36:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: appapi.ironscales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.ironscales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ironscales.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/security/ironscales-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Security
- Cybersecurity
- Phishing
- Anti-Phishing
- Business Email Compromise
- Account Takeover
- Threat Intelligence
- Incident Response
- Security Awareness Training
- Phishing Simulation
- Microsoft-365
- Google Workspace
- SOC Automation
- Deepfake Detection
- MCP
---
