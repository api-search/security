---
api_specs:
- filename: morning-consult-ai-api-openapi.yml
  format: yaml
  label: Morning Consult AI API
  slug: morning-consult-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/openapi/morning-consult-ai-api-openapi.yml
- filename: morning-consult-authentication-api-openapi.yml
  format: yaml
  label: Morning Consult Authentication API
  slug: morning-consult-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/openapi/morning-consult-authentication-api-openapi.yml
- filename: morning-consult-data-api-openapi.yml
  format: yaml
  label: Morning Consult Data API
  slug: morning-consult-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/openapi/morning-consult-data-api-openapi.yml
- filename: morning-consult-lookup-api-openapi.yml
  format: yaml
  label: Morning Consult Lookup API
  slug: morning-consult-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/openapi/morning-consult-lookup-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issuewild "starfieldtech.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: morningconsult.com
  spf: true
hosts:
- cert_expires: Oct  3 18:44:46 2026 GMT
  host: morningconsult.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 01:36:09 2026 GMT
  host: api.morningconsult.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morning Consult Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morning Consult, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Morning Consult
provider_slug: morning-consult
slug: morning-consult-domain-security
source_filename: morning-consult-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morningconsult.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.morningconsult.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:36:09 2026 GMT\n  hsts: null\ndomains:\n- domain: morningconsult.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morning-consult/refs/heads/main/security/morning-consult-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Research
- Survey Data
- Consumer Intelligence
- Brand Tracking
- Decision Intelligence
- Public Opinion
- Analytics
- Data
- Artificial Intelligence
---
