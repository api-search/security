---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Ninetailed Experience API
  slug: ninetailed-experience-api
  spec_type: OpenAPI
  url: https://www.contentful.com/developers/docs/ninetailed/experience-api/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contentful.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ninetailed.co
  spf: false
hosts:
- cert_expires: Sep 22 13:18:24 2026 GMT
  host: www.contentful.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 05:04:04 2026 GMT
  host: experience.ninetailed.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ninetailed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninetailed, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ninetailed
provider_slug: ninetailed
slug: ninetailed-domain-security
source_filename: ninetailed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contentful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: experience.ninetailed.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:04:04 2026 GMT\n  hsts: null\ndomains:\n- domain: contentful.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ninetailed.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninetailed/refs/heads/main/security/ninetailed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Personalization
- Experimentation
- A/B Testing
- Audience Segmentation
- Feature Flags
- Headless CMS
- Edge Computing
- Content Management
---
