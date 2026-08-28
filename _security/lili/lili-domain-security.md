---
api_specs:
- filename: lili-application-api-openapi.yml
  format: yaml
  label: Lili Application API
  slug: lili-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-application-api-openapi.yml
- filename: lili-customer-management-api-openapi.yml
  format: yaml
  label: Lili Customer Management API
  slug: lili-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-customer-management-api-openapi.yml
- filename: lili-webhooks-api-openapi.yml
  format: yaml
  label: Lili Webhooks API
  slug: lili-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:compliance@lili.co"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lili.co
  spf: true
hosts:
- cert_expires: Nov 13 06:22:02 2026 GMT
  host: lili.co
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 07:05:54 2026 GMT
  host: dev.lili.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: prod.lili.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lili Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lili, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lili
provider_slug: lili
slug: lili-domain-security
source_filename: lili-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lili.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 06:22:02 2026 GMT\n  hsts: true\n- host: dev.lili.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 07:05:54 2026 GMT\n  hsts: false\n- host: prod.lili.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lili.co\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:compliance@lili.co\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/security/lili-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Business Banking
- Financial Services
- Fintech
- Embedded Finance
- Onboarding
- KYC
- Webhooks
- MCP
- agent-native
- Invoicing
- Bill Pay
- Accounting
- Small Business
---
