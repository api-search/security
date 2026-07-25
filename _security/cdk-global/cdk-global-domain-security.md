---
api_specs:
- filename: fortellis-event-relay-data-plane-proxy-asyncapi.yml
  format: yaml
  label: Fortellis Event Relay Data Plane Proxy (AsyncAPI)
  slug: fortellis-event-relay-data-plane
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-event-relay-data-plane-proxy-asyncapi.yml
- filename: fortellis-hello-world-asyncapi.yml
  format: yaml
  label: Fortellis AsyncAPI Hello World Reference
  slug: fortellis-async-hello-world
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-hello-world-asyncapi.yml
- filename: cdk-global-adopt-api-openapi.yml
  format: yaml
  label: CDK Global adopt API
  slug: cdk-global-adopt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-adopt-api-openapi.yml
- filename: cdk-global-adopt-delete-api-openapi.yml
  format: yaml
  label: CDK Global adopt delete API
  slug: cdk-global-adopt-delete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-adopt-delete-api-openapi.yml
- filename: cdk-global-adopt-update-api-openapi.yml
  format: yaml
  label: CDK Global adopt update API
  slug: cdk-global-adopt-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-adopt-update-api-openapi.yml
- filename: cdk-global-cancel-api-openapi.yml
  format: yaml
  label: CDK Global cancel API
  slug: cdk-global-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-cancel-api-openapi.yml
- filename: cdk-global-create-api-openapi.yml
  format: yaml
  label: CDK Global create API
  slug: cdk-global-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-create-api-openapi.yml
- filename: cdk-global-events-api-openapi.yml
  format: yaml
  label: CDK Global events API
  slug: cdk-global-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-events-api-openapi.yml
- filename: cdk-global-manage-api-openapi.yml
  format: yaml
  label: CDK Global manage API
  slug: cdk-global-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-manage-api-openapi.yml
- filename: cdk-global-query-api-openapi.yml
  format: yaml
  label: CDK Global query API
  slug: cdk-global-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-query-api-openapi.yml
- filename: cdk-global-service-booking-api-openapi.yml
  format: yaml
  label: CDK Global Service Booking API
  slug: cdk-global-service-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-service-booking-api-openapi.yml
- filename: cdk-global-update-api-openapi.yml
  format: yaml
  label: CDK Global update API
  slug: cdk-global-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/cdk-global-update-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "domainadmin@cdk.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cdkglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fortellis.io
  spf: true
hosts:
- cert_expires: Aug 31 06:56:02 2026 GMT
  host: www.cdkglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:58:35 2026 GMT
  host: fortellis.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.fortellis.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cdk Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CDK Global, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CDK Global
provider_slug: cdk-global
slug: cdk-global-domain-security
source_filename: cdk-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdkglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:56:02 2026 GMT\n  hsts: false\n- host: fortellis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:58:35 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.fortellis.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cdkglobal.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"domainadmin@cdk.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fortellis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/security/cdk-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Dealer Management
- DMS
- Auto Retail
- F&I
- Fixed Operations
- Parts
- CRM
- Digital Retail
- Marketplace
- Developer Platform
- Events
- Webhooks
- AsyncAPI
---
