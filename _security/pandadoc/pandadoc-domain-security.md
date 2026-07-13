---
api_specs:
- filename: pandadoc-rest-api-openapi.yml
  format: yaml
  label: PandaDoc REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-rest-api-openapi.yml
- filename: pandadoc-rest-api-openapi.yml
  format: yaml
  label: PandaDoc Document Generation API
  slug: document-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-rest-api-openapi.yml
- filename: pandadoc-rest-api-openapi.yml
  format: yaml
  label: PandaDoc E-Signature API
  slug: e-signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-rest-api-openapi.yml
- filename: pandadoc-rest-api-openapi.yml
  format: yaml
  label: PandaDoc Embedded Editing API
  slug: embedded-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-rest-api-openapi.yml
- filename: pandadoc-rest-api-openapi.yml
  format: yaml
  label: PandaDoc Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pandadoc.com
  spf: true
hosts:
- cert_expires: Oct  2 13:38:29 2026 GMT
  host: developers.pandadoc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 13:43:11 2026 GMT
  host: www.pandadoc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 19 07:30:46 2026 GMT
  host: api.pandadoc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pandadoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PandaDoc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PandaDoc
provider_slug: pandadoc
slug: pandadoc-domain-security
source_filename: pandadoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.pandadoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:38:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.pandadoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:43:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pandadoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 07:30:46 2026 GMT\n  hsts: null\ndomains:\n- domain: pandadoc.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/security/pandadoc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Automation
- E-Signature
- Document Management
- Document Generation
- Webhooks
---
