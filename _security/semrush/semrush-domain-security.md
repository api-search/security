---
api_specs:
- filename: semrush-hermes-partner-api-api-openapi.yml
  format: yaml
  label: Semrush Hermes Partner API API
  slug: semrush-hermes-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-hermes-partner-api-api-openapi.yml
- filename: semrush-jwt-issuer-api-openapi.yml
  format: yaml
  label: Semrush JWT Issuer API
  slug: semrush-jwt-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-jwt-issuer-api-openapi.yml
- filename: semrush-partner-service-api-openapi.yml
  format: yaml
  label: Semrush Partner Service API
  slug: semrush-partner-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-partner-service-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "comodoca.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: semrush.com
  spf: true
hosts:
- cert_expires: Oct 13 12:08:50 2026 GMT
  host: developer.semrush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 17:30:30 2026 GMT
  host: api.semrush.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Semrush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semrush, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Semrush
provider_slug: semrush
slug: semrush-domain-security
source_filename: semrush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.semrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 12:08:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.semrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:30:30 2026 GMT\n  hsts: null\ndomains:\n- domain: semrush.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/security/semrush-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Search Engines
- SEO
- Marketing
- Marketing Intelligence
- Content Marketing
- Advertising
- Competitive Intelligence
- Keyword Research
- Backlinks
- Rank Tracking
- AI Search Visibility
- Local SEO
- MCP
---
