---
api_specs:
- filename: root-applications-api-openapi.yml
  format: yaml
  label: Root Insurance Applications API
  slug: root-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-applications-api-openapi.yml
- filename: root-calls-api-openapi.yml
  format: yaml
  label: Root Insurance Calls API
  slug: root-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-calls-api-openapi.yml
- filename: root-claims-api-openapi.yml
  format: yaml
  label: Root Insurance Claims API
  slug: root-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-claims-api-openapi.yml
- filename: root-complaints-api-openapi.yml
  format: yaml
  label: Root Insurance Complaints API
  slug: root-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-complaints-api-openapi.yml
- filename: root-data-exports-api-openapi.yml
  format: yaml
  label: Root Insurance Data exports API
  slug: root-data-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-data-exports-api-openapi.yml
- filename: root-data-stores-api-openapi.yml
  format: yaml
  label: Root Insurance Data stores API
  slug: root-data-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-data-stores-api-openapi.yml
- filename: root-embed-api-openapi.yml
  format: yaml
  label: Root Insurance Embed API
  slug: root-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-embed-api-openapi.yml
- filename: root-files-api-openapi.yml
  format: yaml
  label: Root Insurance Files API
  slug: root-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-files-api-openapi.yml
- filename: root-leads-api-openapi.yml
  format: yaml
  label: Root Insurance Leads API
  slug: root-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-leads-api-openapi.yml
- filename: root-notifications-api-openapi.yml
  format: yaml
  label: Root Insurance Notifications API
  slug: root-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-notifications-api-openapi.yml
- filename: root-payment-methods-api-openapi.yml
  format: yaml
  label: Root Insurance Payment Methods API
  slug: root-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-payment-methods-api-openapi.yml
- filename: root-payments-api-openapi.yml
  format: yaml
  label: Root Insurance Payments API
  slug: root-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-payments-api-openapi.yml
- filename: root-policies-api-openapi.yml
  format: yaml
  label: Root Insurance Policies API
  slug: root-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-policies-api-openapi.yml
- filename: root-policyholders-api-openapi.yml
  format: yaml
  label: Root Insurance Policyholders API
  slug: root-policyholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-policyholders-api-openapi.yml
- filename: root-quotes-api-openapi.yml
  format: yaml
  label: Root Insurance Quotes API
  slug: root-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-quotes-api-openapi.yml
- filename: root-secret-keys-api-openapi.yml
  format: yaml
  label: Root Insurance Secret keys API
  slug: root-secret-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-secret-keys-api-openapi.yml
- filename: root-webhooks-api-openapi.yml
  format: yaml
  label: Root Insurance Webhooks API
  slug: root-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinroot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rootplatform.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.joinroot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:10:36 2026 GMT
  host: docs.rootplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.rootplatform.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Root Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Root Insurance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Root Insurance
provider_slug: root
slug: root-domain-security
source_filename: root-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinroot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.rootplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rootplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: joinroot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rootplatform.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/security/root-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Auto Insurance
- Telematics
- Embedded Insurance
- Policy Administration
- Claims
- Usage-Based Insurance
- InsurTech
---
