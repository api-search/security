---
api_specs:
- filename: fortellis-appointments-openapi.yml
  format: yaml
  label: Fortellis Service Appointments API
  slug: fortellis-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-appointments-openapi.yml
- filename: fortellis-user-service-openapi.yml
  format: yaml
  label: Fortellis User / Booking Sessions API
  slug: fortellis-user-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-user-service-openapi.yml
- filename: fortellis-parts-store-openapi.yml
  format: yaml
  label: Fortellis Parts Store API
  slug: fortellis-parts-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-parts-store-openapi.yml
- filename: fortellis-pet-adoption-openapi.yml
  format: yaml
  label: Fortellis Reference Pet Adoption API
  slug: fortellis-pet-adoption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-pet-adoption-openapi.yml
- filename: fortellis-event-relay-webhook-openapi.yml
  format: yaml
  label: Fortellis Event Relay Webhook
  slug: fortellis-event-relay-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-event-relay-webhook-openapi.yml
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
