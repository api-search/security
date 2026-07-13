---
api_specs:
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Analyze Agreements API
  slug: linksquares-analyze-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Analyze Metadata and Smart Values API
  slug: linksquares-analyze-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Finalize Workflow API
  slug: linksquares-finalize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linksquares.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mail.zendesk.com include:amazonses.com include:_spf.salesforce.com include:6934676.spf56.hubspotemail.net include:stspg-customer.com ~all
hosts:
- cert_expires: Sep 20 16:14:10 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: linksquares.com
  hsts: true
  hsts_max_age: 63072000
  http_status: 200
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: api.linksquares.com
  hsts: false
  http_status: 403
  https: true
  note: Production API gateway. Returns 403 without a valid x-api-key header, as expected for a customer-gated API. HSTS header not present on the 403 gateway response.
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: developer.linksquares.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: Interactive developer/API reference portal (login-gated).
  server: nginx
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Linksquares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkSquares, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LinkSquares
provider_slug: linksquares
slug: linksquares-domain-security
source_filename: linksquares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linksquares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Sep 20 16:14:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: cloudflare\n  http_status: 200\n- host: api.linksquares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M04\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n  http_status: 403\n  note: >-\n    Production API gateway. Returns 403 without a valid x-api-key header, as\n    expected for a customer-gated API. HSTS header not present on the 403 gateway\n    response.\n- host: developer.linksquares.com\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: Amazon RSA 2048 M04\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: nginx\n  http_status: 200\n  note: Interactive\
  \ developer/API reference portal (login-gated).\ndomains:\n- domain: linksquares.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:mail.zendesk.com include:amazonses.com include:_spf.salesforce.com include:6934676.spf56.hubspotemail.net include:stspg-customer.com ~all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/security/linksquares-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- AI
- Legal
- Agreements
- Document Management
- Contract Analytics
---
