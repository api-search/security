---
api_specs:
- filename: builtwith-domain-openapi.yml
  format: yaml
  label: BuiltWith Domain API
  slug: builtwith-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-openapi.yml
- filename: builtwith-lists-openapi.yml
  format: yaml
  label: BuiltWith Lists API
  slug: builtwith-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-lists-openapi.yml
- filename: builtwith-trends-openapi.yml
  format: yaml
  label: BuiltWith Trends API
  slug: builtwith-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-trends-openapi.yml
- filename: builtwith-change-openapi.yml
  format: yaml
  label: BuiltWith Change API
  slug: builtwith-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-change-openapi.yml
- filename: builtwith-relationships-openapi.yml
  format: yaml
  label: BuiltWith Relationships API
  slug: builtwith-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-relationships-openapi.yml
- filename: builtwith-free-openapi.yml
  format: yaml
  label: BuiltWith Free API
  slug: builtwith-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-free-openapi.yml
- filename: builtwith-tags-openapi.yml
  format: yaml
  label: BuiltWith Tags API
  slug: builtwith-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-tags-openapi.yml
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
