---
api_specs:
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Customers API
  slug: drycleancloud-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Orders API
  slug: drycleancloud-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Products & Inventory API
  slug: drycleancloud-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Pickup & Delivery API
  slug: drycleancloud-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Payments & Promotions API
  slug: drycleancloud-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Business & Reporting API
  slug: drycleancloud-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Messaging API
  slug: drycleancloud-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Webhooks
  slug: drycleancloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cleancloudapp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cleancloud.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: cleancloudapp.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 13:46:35 2026 GMT
  host: help.cleancloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drycleancloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CleanCloud, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CleanCloud
provider_slug: drycleancloud
slug: drycleancloud-domain-security
source_filename: drycleancloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleancloudapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: help.cleancloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cleancloudapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cleancloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/security/drycleancloud-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Dry Cleaning
- Laundry
- Point of Sale
- POS
- Field Service
- Pickup and Delivery
- SMB Software
---
