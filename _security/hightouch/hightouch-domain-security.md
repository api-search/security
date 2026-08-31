---
api_specs:
- filename: hightouch-sources-api-openapi.yml
  format: yaml
  label: Hightouch Sources API
  slug: hightouch-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-sources-api-openapi.yml
- filename: hightouch-models-api-openapi.yml
  format: yaml
  label: Hightouch Models API
  slug: hightouch-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-models-api-openapi.yml
- filename: hightouch-destinations-api-openapi.yml
  format: yaml
  label: Hightouch Destinations API
  slug: hightouch-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-destinations-api-openapi.yml
- filename: hightouch-syncs-api-openapi.yml
  format: yaml
  label: Hightouch Syncs API
  slug: hightouch-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-syncs-api-openapi.yml
- filename: hightouch-campaigns-api-openapi.yml
  format: yaml
  label: Hightouch Campaigns API
  slug: hightouch-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-campaigns-api-openapi.yml
- filename: hightouch-ai-decisioning-api-openapi.yml
  format: yaml
  label: Hightouch AI Decisioning API
  slug: hightouch-ai-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-ai-decisioning-api-openapi.yml
- filename: hightouch-events-api-openapi.yml
  format: yaml
  label: Hightouch Events API
  slug: hightouch-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-events-api-openapi.yml
- filename: hightouch-identity-resolution-api-openapi.yml
  format: yaml
  label: Hightouch Identity Resolution API
  slug: hightouch-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-identity-resolution-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hightouch.com
  spf: true
hosts:
- cert_expires: Oct 13 07:15:20 2026 GMT
  host: hightouch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: api.hightouch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hightouch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hightouch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hightouch
provider_slug: hightouch
slug: hightouch-domain-security
source_filename: hightouch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hightouch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:15:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hightouch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hightouch.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/security/hightouch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDP
- Data Activation
- Reverse ETL
- Audience Management
- Identity Resolution
- Event Collection
- Marketing
- Advertising
- AI Agents
- Data Warehouse
---
