---
api_specs:
- filename: openapi.json
  format: json
  label: TIBCO Cloud Integration API
  slug: tibco-cloud-integration-api
  spec_type: OpenAPI
  url: https://integration.cloud.tibco.com/docs/api/openapi.json
- filename: io-docs
  format: yaml
  label: TIBCO Mashery API Management
  slug: tibco-mashery-api-management
  spec_type: OpenAPI
  url: https://developer.mashery.com/io-docs
- filename: tibco-businessevents-openapi.yml
  format: yaml
  label: TIBCO BusinessEvents API
  slug: tibco-businessevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/openapi/tibco-businessevents-openapi.yml
- filename: tibco-messaging-asyncapi.yml
  format: yaml
  label: TIBCO Messaging API
  slug: tibco-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/asyncapi/tibco-messaging-asyncapi.yml
- filename: tibco-spotfire-openapi.yml
  format: yaml
  label: TIBCO Spotfire Analytics API
  slug: tibco-spotfire-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/openapi/tibco-spotfire-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tibco.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: developer.tibco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: integration.cloud.tibco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.tibco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tibco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIBCO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TIBCO
provider_slug: tibco
slug: tibco-domain-security
source_filename: tibco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tibco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: integration.cloud.tibco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.tibco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tibco.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/security/tibco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- API Management
- Cloud
- Enterprise Software
- Integration
- Messaging
- Real-Time Data
---
