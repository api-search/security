---
api_specs:
- filename: permutive-cohorts-api-openapi.yml
  format: yaml
  label: Permutive Cohorts API
  slug: permutive-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-cohorts-api-openapi.yml
- filename: permutive-contextual-api-openapi.yml
  format: yaml
  label: Permutive Contextual API
  slug: permutive-contextual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-contextual-api-openapi.yml
- filename: permutive-events-api-openapi.yml
  format: yaml
  label: Permutive Events API
  slug: permutive-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-events-api-openapi.yml
- filename: permutive-identity-api-openapi.yml
  format: yaml
  label: Permutive Identity API
  slug: permutive-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-identity-api-openapi.yml
- filename: permutive-segmentation-api-openapi.yml
  format: yaml
  label: Permutive Segmentation API
  slug: permutive-segmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-segmentation-api-openapi.yml
- filename: permutive-taxonomy-api-openapi.yml
  format: yaml
  label: Permutive Taxonomy API
  slug: permutive-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: permutive.com
  spf: true
hosts:
- cert_expires: Aug 25 12:10:02 2026 GMT
  host: permutive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 03:15:31 2026 GMT
  host: api.permutive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Permutive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Permutive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Permutive
provider_slug: permutive
slug: permutive-domain-security
source_filename: permutive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: permutive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:10:02 2026 GMT\n  hsts: false\n- host: api.permutive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:15:31 2026 GMT\n  hsts: null\ndomains:\n- domain: permutive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/security/permutive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Publishing
- Advertising
- AdTech
- MarTech
- Audience
- Data Collaboration
- Data Management Platform
- Contextual
- Identity
---
