---
api_specs:
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Campaigns API
  slug: donorbox-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Donations API
  slug: donorbox-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Plans API
  slug: donorbox-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Donors API
  slug: donorbox-donors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Events API
  slug: donorbox-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Tickets API
  slug: donorbox-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Event Ticket Purchases API
  slug: donorbox-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: donorbox.org
  spf: true
hosts:
- cert_expires: Oct  3 09:46:14 2026 GMT
  host: donorbox.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Donorbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donorbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Donorbox
provider_slug: donorbox
slug: donorbox-domain-security
source_filename: donorbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donorbox.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:46:14 2026 GMT\n  hsts: false\ndomains:\n- domain: donorbox.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/security/donorbox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Nonprofit
- Fundraising
- Donations
- Payments
- Recurring Giving
- Event Ticketing
---
