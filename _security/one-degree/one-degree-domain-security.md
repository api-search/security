---
api_specs:
- filename: one-degree-housing-api-openapi.yml
  format: yaml
  label: One Degree Housing API
  slug: one-degree-housing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-housing-api-openapi.yml
- filename: one-degree-locations-api-openapi.yml
  format: yaml
  label: One Degree Locations API
  slug: one-degree-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-locations-api-openapi.yml
- filename: one-degree-opportunities-api-openapi.yml
  format: yaml
  label: One Degree Opportunities API
  slug: one-degree-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-opportunities-api-openapi.yml
- filename: one-degree-organizations-api-openapi.yml
  format: yaml
  label: One Degree Organizations API
  slug: one-degree-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-organizations-api-openapi.yml
- filename: one-degree-reference-api-openapi.yml
  format: yaml
  label: One Degree Reference API
  slug: one-degree-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-reference-api-openapi.yml
- filename: one-degree-submissions-api-openapi.yml
  format: yaml
  label: One Degree Submissions API
  slug: one-degree-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1degree.org
  spf: true
hosts:
- cert_expires: Aug 25 03:53:20 2026 GMT
  host: www.1degree.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: data.1degree.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: One Degree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Degree, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: One Degree
provider_slug: one-degree
slug: one-degree-domain-security
source_filename: one-degree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1degree.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 03:53:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.1degree.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 1degree.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/security/one-degree-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Non-Profit
- Social Services
- Community Resources
- Human Services
- Public Benefit
- Housing
- Open Data
- Civic Tech
---
