---
api_specs:
- filename: availity-eligibility-openapi.yml
  format: yaml
  label: Availity Eligibility & Benefits API
  slug: availity-eligibility-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-eligibility-openapi.yml
- filename: availity-claim-status-openapi.yml
  format: yaml
  label: Availity Claim Status API
  slug: availity-claims-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-status-openapi.yml
- filename: availity-claim-attachments-openapi.yml
  format: yaml
  label: Availity Claim Attachments API
  slug: availity-claim-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-attachments-openapi.yml
- filename: availity-service-reviews-openapi.yml
  format: yaml
  label: Availity Service Reviews (Prior Authorization) API
  slug: availity-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-service-reviews-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: availity.com
  spf: true
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: developer.availity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: api.availity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Availity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for availity, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: availity
provider_slug: availity
slug: availity-domain-security
source_filename: availity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.availity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: api.availity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: availity.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/security/availity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
