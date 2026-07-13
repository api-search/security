---
api_specs:
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Customers API
  slug: joblogic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Contacts API
  slug: joblogic-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Sites API
  slug: joblogic-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Assets API
  slug: joblogic-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Jobs API
  slug: joblogic-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Visits API
  slug: joblogic-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Engineers API
  slug: joblogic-engineers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Quotes API
  slug: joblogic-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Invoices API
  slug: joblogic-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joblogic.com
  spf: true
hosts:
- cert_expires: Sep 16 08:00:14 2026 GMT
  host: joblogic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 13:24:22 2026 GMT
  host: api.joblogic.com
  hsts: false
  http_status: 403
  https: true
  note: Production API host resolves and serves TLS but returns 403 - access is firewall / IP-allowlisted per Joblogic's customer-provisioned access model.
  tls_version: TLSv1.3
- cert_expires: Oct 31 06:52:13 2026 GMT
  host: uatapi.joblogic.com
  hsts: false
  http_status: 403
  https: true
  note: UAT sandbox API host; also IP-allowlisted.
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:47:18 2026 GMT
  host: apidocs.joblogic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Public API documentation (Postman-hosted).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joblogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joblogic, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Joblogic
provider_slug: joblogic
slug: joblogic-domain-security
source_filename: joblogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joblogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.joblogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 13:24:22 2026 GMT\n  hsts: false\n  http_status: 403\n  note: Production API host resolves and serves TLS but returns 403 - access is firewall / IP-allowlisted per Joblogic's customer-provisioned access model.\n- host: uatapi.joblogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 06:52:13 2026 GMT\n  hsts: false\n  http_status: 403\n  note: UAT sandbox API host; also IP-allowlisted.\n- host: apidocs.joblogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Public API documentation (Postman-hosted).\ndomains:\n- domain: joblogic.com\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/security/joblogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Job Management
- Scheduling
- Maintenance
- Workforce
- Mobile Workforce
- Trades
- CRM
- SaaS
---
