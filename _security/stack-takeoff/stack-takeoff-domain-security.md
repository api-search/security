---
api_specs:
- filename: stack-takeoff-openapi.yml
  format: yaml
  label: STACK Projects API
  slug: stack-takeoff-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/openapi/stack-takeoff-openapi.yml
- filename: stack-takeoff-openapi.yml
  format: yaml
  label: STACK Plans & Files API
  slug: stack-takeoff-plans-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/openapi/stack-takeoff-openapi.yml
- filename: stack-takeoff-openapi.yml
  format: yaml
  label: STACK Takeoffs API
  slug: stack-takeoff-takeoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/openapi/stack-takeoff-openapi.yml
- filename: stack-takeoff-openapi.yml
  format: yaml
  label: STACK Estimates API
  slug: stack-takeoff-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/openapi/stack-takeoff-openapi.yml
- filename: stack-takeoff-openapi.yml
  format: yaml
  label: STACK Items & Assemblies API
  slug: stack-takeoff-items-assemblies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/openapi/stack-takeoff-openapi.yml
- filename: stack-takeoff-openapi.yml
  format: yaml
  label: STACK Reference Data API
  slug: stack-takeoff-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/openapi/stack-takeoff-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackct.com
  spf: true
hosts:
- cert_expires: Sep 24 10:09:19 2026 GMT
  host: www.stackct.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stack Takeoff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STACK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: STACK
provider_slug: stack-takeoff
slug: stack-takeoff-domain-security
source_filename: stack-takeoff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:09:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stackct.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/security/stack-takeoff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Preconstruction
- Takeoff
- Estimating
- Construction Technology
- Partner API
---
