---
api_specs:
- filename: kili-technology-openapi.yml
  format: yaml
  label: Kili Technology Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/openapi/kili-technology-openapi.yml
- filename: kili-technology-openapi.yml
  format: yaml
  label: Kili Technology Assets API
  slug: assets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/openapi/kili-technology-openapi.yml
- filename: kili-technology-openapi.yml
  format: yaml
  label: Kili Technology Labels API
  slug: labels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/openapi/kili-technology-openapi.yml
- filename: kili-technology-openapi.yml
  format: yaml
  label: Kili Technology Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/openapi/kili-technology-openapi.yml
- filename: kili-technology-openapi.yml
  format: yaml
  label: Kili Technology Users API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/openapi/kili-technology-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kili-technology.com
  spf: true
hosts:
- cert_expires: Sep 26 10:01:15 2026 GMT
  host: kili-technology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:00:56 2026 GMT
  host: docs.kili-technology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 22:04:23 2026 GMT
  host: cloud.kili-technology.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kili Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kili Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kili Technology
provider_slug: kili-technology
slug: kili-technology-domain-security
source_filename: kili-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kili-technology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:01:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kili-technology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:00:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.kili-technology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:04:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kili-technology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/security/kili-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Data Labeling
- Training Data
- Annotation
- GraphQL
---
