---
api_specs:
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Field and Metadata Extraction API
  slug: field-extraction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Workflow API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evisort.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.evisort.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 14:25:03 2026 GMT
  host: documents.developers.evisort.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 04:43:27 2026 GMT
  host: api.evisort.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evisort Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evisort, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Evisort
provider_slug: evisort
slug: evisort-domain-security
source_filename: evisort-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evisort.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documents.developers.evisort.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:25:03 2026 GMT\n  hsts: null\n- host: api.evisort.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:43:27 2026 GMT\n  hsts: null\ndomains:\n- domain: evisort.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/security/evisort-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Contract Lifecycle Management
- CLM
- Contract Intelligence
- Document AI
- Legal Tech
---
