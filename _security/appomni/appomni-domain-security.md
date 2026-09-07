---
api_specs:
- filename: appomni-security-events-api-openapi.yml
  format: yaml
  label: AppOmni Posture Findings API
  slug: appomni-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-security-events-api-openapi.yml
- filename: appomni-policies-api-openapi.yml
  format: yaml
  label: AppOmni Policies API
  slug: appomni-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-policies-api-openapi.yml
- filename: appomni-compliance-api-openapi.yml
  format: yaml
  label: AppOmni Compliance and Reports API
  slug: appomni-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-compliance-api-openapi.yml
- filename: appomni-monitored-services-api-openapi.yml
  format: yaml
  label: AppOmni Monitored Services API
  slug: appomni-monitored-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-monitored-services-api-openapi.yml
- filename: appomni-identity-api-openapi.yml
  format: yaml
  label: AppOmni Identity and Access API
  slug: appomni-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-identity-api-openapi.yml
- filename: appomni-scim-api-openapi.yml
  format: yaml
  label: AppOmni SCIM 2.0 API
  slug: appomni-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-scim-api-openapi.yml
- filename: appomni-discovery-insights-api-openapi.yml
  format: yaml
  label: AppOmni Discovery, Insights and Audit API
  slug: appomni-discovery-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-discovery-insights-api-openapi.yml
- filename: appomni-developer-platform-api-openapi.yml
  format: yaml
  label: AppOmni Developer Platform API
  slug: appomni-developer-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-developer-platform-api-openapi.yml
- filename: appomni-ai-api-openapi.yml
  format: yaml
  label: AppOmni AI API
  slug: appomni-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-ai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appomni.com
  spf: true
hosts:
- cert_expires: Nov 12 21:32:17 2026 GMT
  host: appomni.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 05:22:02 2026 GMT
  host: api.appomni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Appomni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppOmni, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppOmni
provider_slug: appomni
slug: appomni-domain-security
source_filename: appomni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appomni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 21:32:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: api.appomni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 05:22:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appomni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/security/appomni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS Security
- SSPM
- Compliance
- Threat Detection
- CASB
- Zero Trust
- Identity
- SCIM
- AI Security
- Posture Management
---
