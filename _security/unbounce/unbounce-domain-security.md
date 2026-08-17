---
api_specs:
- filename: unbounce-accounts-api-openapi.yml
  format: yaml
  label: Unbounce Accounts API
  slug: unbounce-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-accounts-api-openapi.yml
- filename: unbounce-domains-api-openapi.yml
  format: yaml
  label: Unbounce Domains API
  slug: unbounce-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-domains-api-openapi.yml
- filename: unbounce-leads-api-openapi.yml
  format: yaml
  label: Unbounce Leads API
  slug: unbounce-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-leads-api-openapi.yml
- filename: unbounce-meta-api-openapi.yml
  format: yaml
  label: Unbounce Meta API
  slug: unbounce-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-meta-api-openapi.yml
- filename: unbounce-pagegroups-api-openapi.yml
  format: yaml
  label: Unbounce PageGroups API
  slug: unbounce-pagegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-pagegroups-api-openapi.yml
- filename: unbounce-pages-api-openapi.yml
  format: yaml
  label: Unbounce Pages API
  slug: unbounce-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-pages-api-openapi.yml
- filename: unbounce-users-api-openapi.yml
  format: yaml
  label: Unbounce Users API
  slug: unbounce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:postmaster+caa-policy@unbounce.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unbounce.com
  spf: true
hosts:
- cert_expires: Oct 24 11:59:54 2026 GMT
  host: unbounce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developer.unbounce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.unbounce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unbounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unbounce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unbounce
provider_slug: unbounce
slug: unbounce-domain-security
source_filename: unbounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 11:59:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.unbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: api.unbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unbounce.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:postmaster+caa-policy@unbounce.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/security/unbounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Landing Pages
- Conversion Rate Optimization
- Marketing
- A/B Testing
- Lead Generation
- Marketing Automation
---
