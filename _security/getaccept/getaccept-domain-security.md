---
api_specs:
- filename: getaccept-archive-api-openapi.yml
  format: yaml
  label: GetAccept Archive API
  slug: getaccept-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-archive-api-openapi.yml
- filename: getaccept-attachments-api-openapi.yml
  format: yaml
  label: GetAccept Attachments API
  slug: getaccept-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-attachments-api-openapi.yml
- filename: getaccept-authentication-api-openapi.yml
  format: yaml
  label: GetAccept Authentication API
  slug: getaccept-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-authentication-api-openapi.yml
- filename: getaccept-communication-templates-api-openapi.yml
  format: yaml
  label: GetAccept Communication Templates API
  slug: getaccept-communication-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-communication-templates-api-openapi.yml
- filename: getaccept-contacts-api-openapi.yml
  format: yaml
  label: GetAccept Contacts API
  slug: getaccept-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-contacts-api-openapi.yml
- filename: getaccept-custom-data-api-openapi.yml
  format: yaml
  label: GetAccept Custom Data API
  slug: getaccept-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-custom-data-api-openapi.yml
- filename: getaccept-documents-api-openapi.yml
  format: yaml
  label: GetAccept Documents API
  slug: getaccept-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-documents-api-openapi.yml
- filename: getaccept-others-api-openapi.yml
  format: yaml
  label: GetAccept Others API
  slug: getaccept-others-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-others-api-openapi.yml
- filename: getaccept-subscriptions-api-openapi.yml
  format: yaml
  label: GetAccept Subscriptions API
  slug: getaccept-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-subscriptions-api-openapi.yml
- filename: getaccept-templates-api-openapi.yml
  format: yaml
  label: GetAccept Templates API
  slug: getaccept-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-templates-api-openapi.yml
- filename: getaccept-users-api-openapi.yml
  format: yaml
  label: GetAccept Users API
  slug: getaccept-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-users-api-openapi.yml
- filename: getaccept-videos-api-openapi.yml
  format: yaml
  label: GetAccept Videos API
  slug: getaccept-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-videos-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "getaccept.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getaccept.com
  spf: true
hosts:
- cert_expires: Sep 22 10:08:27 2026 GMT
  host: www.getaccept.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getaccept Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetAccept, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GetAccept
provider_slug: getaccept
slug: getaccept-domain-security
source_filename: getaccept-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getaccept.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:08:27 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: getaccept.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"getaccept.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/security/getaccept-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Sales Enablement
- Electronic Signature
- E-Signature
- Digital Sales Room
- Document Management
- Contract Management
- Proposals
- SaaS
---
