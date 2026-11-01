---
api_specs:
- filename: ecosio-approval-request-status-api-openapi.yml
  format: yaml
  label: ecosio Approval Request Status API
  slug: ecosio-approval-request-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-approval-request-status-api-openapi.yml
- filename: ecosio-archive-messages-api-openapi.yml
  format: yaml
  label: ecosio Archive messages API
  slug: ecosio-archive-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-archive-messages-api-openapi.yml
- filename: ecosio-check-user-credentials-api-openapi.yml
  format: yaml
  label: ecosio Check user credentials API
  slug: ecosio-check-user-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-check-user-credentials-api-openapi.yml
- filename: ecosio-companies-api-openapi.yml
  format: yaml
  label: ecosio Companies API
  slug: ecosio-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-companies-api-openapi.yml
- filename: ecosio-connectors-api-openapi.yml
  format: yaml
  label: ecosio Connectors API
  slug: ecosio-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-connectors-api-openapi.yml
- filename: ecosio-deliver-messages-to-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Deliver messages to the Hub API
  slug: ecosio-deliver-messages-to-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-deliver-messages-to-the-hub-api-openapi.yml
- filename: ecosio-fetch-messages-from-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Fetch messages from the Hub API
  slug: ecosio-fetch-messages-from-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-fetch-messages-from-the-hub-api-openapi.yml
- filename: ecosio-message-controller-api-openapi.yml
  format: yaml
  label: ecosio Message Controller API
  slug: ecosio-message-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-message-controller-api-openapi.yml
- filename: ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
  format: yaml
  label: ecosio Request the documents for an e-invoice API
  slug: ecosio-request-the-documents-for-an-e-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
- filename: ecosio-scenarios-api-openapi.yml
  format: yaml
  label: ecosio Scenarios API
  slug: ecosio-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-scenarios-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecosio.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecosio-hub.com
  spf: true
hosts:
- cert_expires: Jan  1 14:41:42 2027 GMT
  host: ecosio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  1 23:59:59 2027 GMT
  host: api.test.ecosio-hub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 03:34:37 2026 GMT
  host: e-invoicing-message-qa.platdev.vtxdev.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ecosio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ecosio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ecosio
provider_slug: ecosio
slug: ecosio-domain-security
source_filename: ecosio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecosio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 14:41:42 2027 GMT\n  hsts: null\n- host: api.test.ecosio-hub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 23:59:59 2027 GMT\n  hsts: null\n- host: e-invoicing-message-qa.platdev.vtxdev.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 03:34:37 2026 GMT\n  hsts: null\ndomains:\n- domain: ecosio.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ecosio-hub.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ecosio/security/ecosio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- EDI
- E-Invoicing
- B2B Integration
- VAT Compliance
- PEPPOL
- Supply Chain
- Messaging
---
