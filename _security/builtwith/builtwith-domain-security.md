---
api_specs:
- filename: builtwith-bulk-processing-api-openapi.yml
  format: yaml
  label: BuiltWith Bulk Processing API
  slug: builtwith-bulk-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-bulk-processing-api-openapi.yml
- filename: builtwith-domain-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Domain Lookup API
  slug: builtwith-domain-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-lookup-api-openapi.yml
- filename: builtwith-domain-relationships-api-openapi.yml
  format: yaml
  label: BuiltWith Domain Relationships API
  slug: builtwith-domain-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-relationships-api-openapi.yml
- filename: builtwith-free-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Free Lookup API
  slug: builtwith-free-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-free-lookup-api-openapi.yml
- filename: builtwith-tag-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Tag Lookup API
  slug: builtwith-tag-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-tag-lookup-api-openapi.yml
- filename: builtwith-technology-changes-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Changes API
  slug: builtwith-technology-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-changes-api-openapi.yml
- filename: builtwith-technology-lists-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Lists API
  slug: builtwith-technology-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-lists-api-openapi.yml
- filename: builtwith-technology-trends-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Trends API
  slug: builtwith-technology-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-trends-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:support@builtwith.com"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "symantec.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: builtwith.com
  spf: true
hosts:
- cert_expires: Oct  4 16:38:25 2026 GMT
  host: builtwith.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  6 16:00:28 2026 GMT
  host: api.builtwith.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 24 16:26:05 2026 GMT
  host: sync.builtwith.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Builtwith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuiltWith, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BuiltWith
provider_slug: builtwith
slug: builtwith-domain-security
source_filename: builtwith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: builtwith.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 16:38:25 2026 GMT\n  hsts: false\n- host: api.builtwith.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 16:00:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sync.builtwith.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 16:26:05 2026 GMT\n  hsts: null\ndomains:\n- domain: builtwith.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:support@builtwith.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"symantec.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/security/builtwith-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Technology Profiling
- Lead Generation
- Web Intelligence
- Technology Detection
- Website Analysis
- Market Research
---
