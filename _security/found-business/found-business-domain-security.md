---
api_specs:
- filename: found-business-openapi.yml
  format: yaml
  label: Found Banking
  slug: found-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/found-business/refs/heads/main/openapi/found-business-openapi.yml
- filename: found-business-openapi.yml
  format: yaml
  label: Found Bookkeeping
  slug: found-bookkeeping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/found-business/refs/heads/main/openapi/found-business-openapi.yml
- filename: found-business-openapi.yml
  format: yaml
  label: Found Taxes
  slug: found-taxes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/found-business/refs/heads/main/openapi/found-business-openapi.yml
- filename: found-business-openapi.yml
  format: yaml
  label: Found Invoicing
  slug: found-invoicing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/found-business/refs/heads/main/openapi/found-business-openapi.yml
- filename: found-business-openapi.yml
  format: yaml
  label: Found Contractor Management
  slug: found-contractors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/found-business/refs/heads/main/openapi/found-business-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: found.com
  spf: true
hosts:
- cert_expires: Sep 17 16:01:14 2026 GMT
  host: found.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Found Business Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Found, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Found
provider_slug: found-business
slug: found-business-domain-security
source_filename: found-business-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: found.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:01:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: found.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/found-business/refs/heads/main/security/found-business-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Business Banking
- Bookkeeping
- Taxes
- Self-Employed
---
