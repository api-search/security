---
api_specs:
- filename: knownwell-alignment-api-openapi.yml
  format: yaml
  label: Knownwell alignment API
  slug: knownwell-alignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-alignment-api-openapi.yml
- filename: knownwell-api-keys-api-openapi.yml
  format: yaml
  label: Knownwell api-keys API
  slug: knownwell-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-api-keys-api-openapi.yml
- filename: knownwell-clients-api-openapi.yml
  format: yaml
  label: Knownwell clients API
  slug: knownwell-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-clients-api-openapi.yml
- filename: knownwell-documentation-api-openapi.yml
  format: yaml
  label: Knownwell documentation API
  slug: knownwell-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-documentation-api-openapi.yml
- filename: knownwell-health-api-openapi.yml
  format: yaml
  label: Knownwell health API
  slug: knownwell-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-health-api-openapi.yml
- filename: knownwell-portfolios-api-openapi.yml
  format: yaml
  label: Knownwell portfolios API
  slug: knownwell-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-portfolios-api-openapi.yml
- filename: knownwell-root-api-openapi.yml
  format: yaml
  label: Knownwell root API
  slug: knownwell-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-root-api-openapi.yml
- filename: knownwell-status-api-openapi.yml
  format: yaml
  label: Knownwell status API
  slug: knownwell-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-status-api-openapi.yml
- filename: knownwell-streams-api-openapi.yml
  format: yaml
  label: Knownwell streams API
  slug: knownwell-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-streams-api-openapi.yml
- filename: knownwell-topics-api-openapi.yml
  format: yaml
  label: Knownwell topics API
  slug: knownwell-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knownwell.com
  spf: true
hosts:
- cert_expires: Oct 14 16:46:48 2026 GMT
  host: knownwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 16:33:25 2026 GMT
  host: api.knownwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knownwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knownwell, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knownwell
provider_slug: knownwell
slug: knownwell-domain-security
source_filename: knownwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knownwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:46:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.knownwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 16:33:25 2026 GMT\n  hsts: null\ndomains:\n- domain: knownwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/security/knownwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commercial Intelligence
- Client Intelligence
- Customer Success
- Revenue Operations
- Professional Services
- Artificial Intelligence
- Analytics
- CRM
- Churn Risk
---
