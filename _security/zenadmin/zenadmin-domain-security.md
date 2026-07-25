---
api_specs:
- filename: zenadmin-catalog-api-openapi.yml
  format: yaml
  label: ZenAdmin Catalog API
  slug: zenadmin-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-catalog-api-openapi.yml
- filename: zenadmin-context-api-openapi.yml
  format: yaml
  label: ZenAdmin Context API
  slug: zenadmin-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-context-api-openapi.yml
- filename: zenadmin-devices-api-openapi.yml
  format: yaml
  label: ZenAdmin Devices API
  slug: zenadmin-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-devices-api-openapi.yml
- filename: zenadmin-employees-api-openapi.yml
  format: yaml
  label: ZenAdmin Employees API
  slug: zenadmin-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-employees-api-openapi.yml
- filename: zenadmin-orders-api-openapi.yml
  format: yaml
  label: ZenAdmin Orders API
  slug: zenadmin-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-orders-api-openapi.yml
- filename: zenadmin-webhooks-api-openapi.yml
  format: yaml
  label: ZenAdmin Webhooks API
  slug: zenadmin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:caa@zenadmin.ai"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenadmin.ai
  spf: true
hosts:
- cert_expires: Aug 24 07:34:20 2026 GMT
  host: zenadmin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenadmin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenAdmin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZenAdmin
provider_slug: zenadmin
slug: zenadmin-domain-security
source_filename: zenadmin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenadmin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:34:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zenadmin.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:caa@zenadmin.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/security/zenadmin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT Management
- Device Management
- Mobile Device Management
- IT Asset Management
- SaaS Management
- Identity and Access Management
- IT Procurement
- Employee Lifecycle
- Webhooks
---
