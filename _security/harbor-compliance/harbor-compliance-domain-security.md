---
api_specs:
- filename: harbor-compliance-compliance-filings-api-openapi.yml
  format: yaml
  label: Harbor Compliance Compliance Filings API
  slug: harbor-compliance-compliance-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-compliance-filings-api-openapi.yml
- filename: harbor-compliance-entities-api-openapi.yml
  format: yaml
  label: Harbor Compliance Entities API
  slug: harbor-compliance-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-entities-api-openapi.yml
- filename: harbor-compliance-jurisdictions-api-openapi.yml
  format: yaml
  label: Harbor Compliance Jurisdictions API
  slug: harbor-compliance-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-jurisdictions-api-openapi.yml
- filename: harbor-compliance-licenses-api-openapi.yml
  format: yaml
  label: Harbor Compliance Licenses API
  slug: harbor-compliance-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-licenses-api-openapi.yml
- filename: harbor-compliance-orders-api-openapi.yml
  format: yaml
  label: Harbor Compliance Orders API
  slug: harbor-compliance-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-orders-api-openapi.yml
- filename: harbor-compliance-registered-agents-api-openapi.yml
  format: yaml
  label: Harbor Compliance Registered Agents API
  slug: harbor-compliance-registered-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-registered-agents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: harborcompliance.com
  spf: true
hosts:
- cert_expires: Aug 11 16:18:56 2026 GMT
  host: developers.harborcompliance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.harborcompliance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.harborcompliance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Harbor Compliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harbor Compliance, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Harbor Compliance
provider_slug: harbor-compliance
slug: harbor-compliance-domain-security
source_filename: harbor-compliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.harborcompliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 16:18:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.harborcompliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.harborcompliance.com\n  https: false\ndomains:\n- domain: harborcompliance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/security/harbor-compliance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Licensing
- Compliance
- Legal
- Regulatory
---
