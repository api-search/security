---
api_specs:
- filename: donately-openapi.yml
  format: yaml
  label: Donately Donations API
  slug: donately-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately People API
  slug: donately-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Campaigns API
  slug: donately-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Fundraisers API
  slug: donately-fundraisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Subscriptions API
  slug: donately-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
- filename: donately-openapi.yml
  format: yaml
  label: Donately Accounts API
  slug: donately-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/openapi/donately-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: donately.com
  spf: true
hosts:
- cert_expires: Sep 18 12:51:13 2026 GMT
  host: www.donately.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 17:34:53 2026 GMT
  host: developer.donately.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: api.donately.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Donately Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donately, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Donately
provider_slug: donately
slug: donately-domain-security
source_filename: donately-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.donately.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:51:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.donately.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:34:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.donately.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: donately.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donately/refs/heads/main/security/donately-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fundraising
- Donations
- Nonprofit
- Payments
- Donor Management
- Recurring Giving
---
