---
api_specs:
- filename: jaggaer-async-api-openapi.yml
  format: yaml
  label: JAGGAER Async API
  slug: jaggaer-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-async-api-openapi.yml
- filename: jaggaer-attributes-api-openapi.yml
  format: yaml
  label: JAGGAER Attributes API
  slug: jaggaer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-attributes-api-openapi.yml
- filename: jaggaer-awards-api-openapi.yml
  format: yaml
  label: JAGGAER Awards API
  slug: jaggaer-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-awards-api-openapi.yml
- filename: jaggaer-bids-api-openapi.yml
  format: yaml
  label: JAGGAER Bids API
  slug: jaggaer-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-bids-api-openapi.yml
- filename: jaggaer-contacts-api-openapi.yml
  format: yaml
  label: JAGGAER Contacts API
  slug: jaggaer-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-contacts-api-openapi.yml
- filename: jaggaer-customer-hosts-api-openapi.yml
  format: yaml
  label: JAGGAER Customer Hosts API
  slug: jaggaer-customer-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-customer-hosts-api-openapi.yml
- filename: jaggaer-events-api-openapi.yml
  format: yaml
  label: JAGGAER Events API
  slug: jaggaer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-events-api-openapi.yml
- filename: jaggaer-items-api-openapi.yml
  format: yaml
  label: JAGGAER Items API
  slug: jaggaer-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-items-api-openapi.yml
- filename: jaggaer-jobs-api-openapi.yml
  format: yaml
  label: JAGGAER Jobs API
  slug: jaggaer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-jobs-api-openapi.yml
- filename: jaggaer-locations-api-openapi.yml
  format: yaml
  label: JAGGAER Locations API
  slug: jaggaer-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-locations-api-openapi.yml
- filename: jaggaer-rates-api-openapi.yml
  format: yaml
  label: JAGGAER Rates API
  slug: jaggaer-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-rates-api-openapi.yml
- filename: jaggaer-scenarios-api-openapi.yml
  format: yaml
  label: JAGGAER Scenarios API
  slug: jaggaer-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-scenarios-api-openapi.yml
- filename: jaggaer-suppliers-api-openapi.yml
  format: yaml
  label: JAGGAER Suppliers API
  slug: jaggaer-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-suppliers-api-openapi.yml
- filename: jaggaer-templates-api-openapi.yml
  format: yaml
  label: JAGGAER Templates API
  slug: jaggaer-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-templates-api-openapi.yml
- filename: jaggaer-uploads-api-openapi.yml
  format: yaml
  label: JAGGAER Uploads API
  slug: jaggaer-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-uploads-api-openapi.yml
- filename: jaggaer-users-api-openapi.yml
  format: yaml
  label: JAGGAER Users API
  slug: jaggaer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jaggaer.com
  spf: true
hosts:
- cert_expires: Aug 12 02:41:01 2026 GMT
  host: www.jaggaer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: asodocs.jaggaer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: ches.aso-api.jaggaer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jaggaer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAGGAER, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: JAGGAER
provider_slug: jaggaer
slug: jaggaer-domain-security
source_filename: jaggaer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: asodocs.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ches.aso-api.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jaggaer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/security/jaggaer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Procurement
- Sourcing
- Supplier Management
- Contracts
- Spend Analytics
- eProcurement
- Source-to-Pay
- Procure-to-Pay
---
