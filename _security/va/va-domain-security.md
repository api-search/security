---
api_specs:
- filename: va-appealable-issues-api-openapi.yml
  format: yaml
  label: Veterans Affairs Appealable Issues API
  slug: va-appealable-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-appealable-issues-api-openapi.yml
- filename: va-appeals-status-api-openapi.yml
  format: yaml
  label: Veterans Affairs Appeals Status API
  slug: va-appeals-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-appeals-status-api-openapi.yml
- filename: va-contestable-issues-api-openapi.yml
  format: yaml
  label: Veterans Affairs Contestable Issues API
  slug: va-contestable-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-contestable-issues-api-openapi.yml
- filename: va-higher-level-reviews-api-openapi.yml
  format: yaml
  label: Veterans Affairs Higher-Level Reviews API
  slug: va-higher-level-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-higher-level-reviews-api-openapi.yml
- filename: va-labs-and-tests-api-openapi.yml
  format: yaml
  label: Veterans Affairs Labs And Tests API
  slug: va-labs-and-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-labs-and-tests-api-openapi.yml
- filename: va-legacy-appeals-api-openapi.yml
  format: yaml
  label: Veterans Affairs Legacy Appeals API
  slug: va-legacy-appeals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-legacy-appeals-api-openapi.yml
- filename: va-medical-records-api-openapi.yml
  format: yaml
  label: Veterans Affairs Medical Records API
  slug: va-medical-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-medical-records-api-openapi.yml
- filename: va-messaging-api-openapi.yml
  format: yaml
  label: Veterans Affairs Messaging API
  slug: va-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-messaging-api-openapi.yml
- filename: va-notice-of-disagreements-api-openapi.yml
  format: yaml
  label: Veterans Affairs Notice of Disagreements API
  slug: va-notice-of-disagreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-notice-of-disagreements-api-openapi.yml
- filename: va-other-accredited-representatives-api-openapi.yml
  format: yaml
  label: Veterans Affairs Other Accredited Representatives API
  slug: va-other-accredited-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-other-accredited-representatives-api-openapi.yml
- filename: va-prescriptions-api-openapi.yml
  format: yaml
  label: Veterans Affairs Prescriptions API
  slug: va-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-prescriptions-api-openapi.yml
- filename: va-supplemental-claims-api-openapi.yml
  format: yaml
  label: Veterans Affairs Supplemental Claims API
  slug: va-supplemental-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-supplemental-claims-api-openapi.yml
- filename: va-tooltips-api-openapi.yml
  format: yaml
  label: Veterans Affairs Tooltips API
  slug: va-tooltips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-tooltips-api-openapi.yml
- filename: va-unique-user-metrics-api-openapi.yml
  format: yaml
  label: Veterans Affairs Unique User Metrics API
  slug: va-unique-user-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-unique-user-metrics-api-openapi.yml
- filename: va-vso-accredited-representatives-api-openapi.yml
  format: yaml
  label: Veterans Affairs VSO Accredited Representatives API
  slug: va-vso-accredited-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/openapi/va-vso-accredited-representatives-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: va.gov
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developer.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Va Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veterans Affairs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Veterans Affairs
provider_slug: va
slug: va-domain-security
source_filename: va-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: va.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/security/va-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Veterans
- Government
- Health
- Benefits
- FHIR
- Appeals
- Federal
---
