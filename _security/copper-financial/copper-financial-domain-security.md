---
api_specs:
- filename: copper-financial-account-api-openapi.yml
  format: yaml
  label: Copper Financial Account API
  slug: copper-financial-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-account-api-openapi.yml
- filename: copper-financial-activities-api-openapi.yml
  format: yaml
  label: Copper Financial Activities API
  slug: copper-financial-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-activities-api-openapi.yml
- filename: copper-financial-companies-api-openapi.yml
  format: yaml
  label: Copper Financial Companies API
  slug: copper-financial-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-companies-api-openapi.yml
- filename: copper-financial-custom-fields-api-openapi.yml
  format: yaml
  label: Copper Financial Custom Fields API
  slug: copper-financial-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-custom-fields-api-openapi.yml
- filename: copper-financial-field-layouts-api-openapi.yml
  format: yaml
  label: Copper Financial Field Layouts API
  slug: copper-financial-field-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-field-layouts-api-openapi.yml
- filename: copper-financial-leads-api-openapi.yml
  format: yaml
  label: Copper Financial Leads API
  slug: copper-financial-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-leads-api-openapi.yml
- filename: copper-financial-opportunities-api-openapi.yml
  format: yaml
  label: Copper Financial Opportunities API
  slug: copper-financial-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-opportunities-api-openapi.yml
- filename: copper-financial-people-api-openapi.yml
  format: yaml
  label: Copper Financial People API
  slug: copper-financial-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-people-api-openapi.yml
- filename: copper-financial-related-items-api-openapi.yml
  format: yaml
  label: Copper Financial Related Items API
  slug: copper-financial-related-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-related-items-api-openapi.yml
- filename: copper-financial-tags-api-openapi.yml
  format: yaml
  label: Copper Financial Tags API
  slug: copper-financial-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-tags-api-openapi.yml
- filename: copper-financial-tasks-api-openapi.yml
  format: yaml
  label: Copper Financial Tasks API
  slug: copper-financial-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-tasks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:ops@copper.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: copper.com
  spf: true
hosts:
- cert_expires: Dec 17 01:00:09 2026 GMT
  host: www.copper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Copper Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copper Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Copper Financial
provider_slug: copper-financial
slug: copper-financial-domain-security
source_filename: copper-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.copper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 01:00:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: copper.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ops@copper.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/security/copper-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Software-as-a-Service
- Sales
- Marketing
---
