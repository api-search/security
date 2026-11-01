---
api_specs:
- filename: fundraiseup-donations-api-openapi.yml
  format: yaml
  label: Fundraise Up Donations API
  slug: fundraiseup-donations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-donations-api-openapi.yml
- filename: fundraiseup-events-api-openapi.yml
  format: yaml
  label: Fundraise Up Events API
  slug: fundraiseup-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-events-api-openapi.yml
- filename: fundraiseup-recurring-plans-api-openapi.yml
  format: yaml
  label: Fundraise Up Recurring Plans API
  slug: fundraiseup-recurring-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-recurring-plans-api-openapi.yml
- filename: fundraiseup-supporters-api-openapi.yml
  format: yaml
  label: Fundraise Up Supporters API
  slug: fundraiseup-supporters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-supporters-api-openapi.yml
- filename: fundraiseup-access-links-api-openapi.yml
  format: yaml
  label: Fundraise Up Access links API
  slug: fundraiseup-access-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-access-links-api-openapi.yml
- filename: fundraiseup-campaigns-api-openapi.yml
  format: yaml
  label: Fundraise Up Campaigns API
  slug: fundraiseup-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-campaigns-api-openapi.yml
- filename: fundraiseup-designation-configurations-api-openapi.yml
  format: yaml
  label: Fundraise Up Designation configurations API
  slug: fundraiseup-designation-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-designation-configurations-api-openapi.yml
- filename: fundraiseup-designation-groups-api-openapi.yml
  format: yaml
  label: Fundraise Up Designation groups API
  slug: fundraiseup-designation-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-designation-groups-api-openapi.yml
- filename: fundraiseup-designations-api-openapi.yml
  format: yaml
  label: Fundraise Up Designations API
  slug: fundraiseup-designations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-designations-api-openapi.yml
- filename: fundraiseup-fundraisers-api-openapi.yml
  format: yaml
  label: Fundraise Up Fundraisers API
  slug: fundraiseup-fundraisers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-fundraisers-api-openapi.yml
- filename: fundraiseup-upgrade-links-api-openapi.yml
  format: yaml
  label: Fundraise Up Upgrade links API
  slug: fundraiseup-upgrade-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundraiseup/openapi/fundraiseup-upgrade-links-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fundraiseup.com
  spf: true
hosts:
- cert_expires: Dec 20 14:00:34 2026 GMT
  host: fundraiseup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 14:00:34 2026 GMT
  host: api.fundraiseup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
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
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundraiseup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 14:00:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fundraiseup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 14:00:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fundraiseup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fundraiseup/security/fundraiseup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fundraising
- Donations
- Non-Profit
- Payments
- Recurring Giving
- Donor Management
---
