---
api_specs:
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Donations API
  slug: fundraiseup-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Recurring Plans API
  slug: fundraiseup-recurring-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Supporters API
  slug: fundraiseup-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Events API
  slug: fundraiseup-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Donor Portal Access Links API
  slug: fundraiseup-donor-portal-access-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fundraiseup.com
  spf: true
hosts:
- cert_expires: Sep 14 09:28:36 2026 GMT
  host: fundraiseup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 15:13:34 2026 GMT
  host: api.fundraiseup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fundraiseup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fundraise Up, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fundraise Up
provider_slug: fundraiseup
slug: fundraiseup-domain-security
source_filename: fundraiseup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundraiseup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fundraiseup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fundraiseup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/security/fundraiseup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fundraising
- Donations
- Nonprofit
- Payments
- Recurring Giving
- Donor Management
---
