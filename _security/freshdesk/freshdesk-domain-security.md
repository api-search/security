---
api_specs:
- filename: freshdesk-rest-api-openapi.yml
  format: yaml
  label: Freshdesk REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/openapi/freshdesk-rest-api-openapi.yml
- filename: freshdesk-webhook-api-asyncapi.yml
  format: yaml
  label: Freshdesk Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/asyncapi/freshdesk-webhook-api-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freshdesk.com
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: developers.freshdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:44:14 2026 GMT
  host: yourdomain.freshdesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:44:14 2026 GMT
  host: support.freshdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for freshdesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: freshdesk
provider_slug: freshdesk
slug: freshdesk-domain-security
source_filename: freshdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourdomain.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:44:14 2026 GMT\n  hsts: null\n- host: support.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshdesk.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshdesk/refs/heads/main/security/freshdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
