---
api_specs:
- filename: packback-openapi.yml
  format: yaml
  label: Packback Questions / Discussions
  slug: questions-discussions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packback/refs/heads/main/openapi/packback-openapi.yml
- filename: packback-openapi.yml
  format: yaml
  label: Packback Writing / Deep Dives
  slug: writing-deep-dives
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packback/refs/heads/main/openapi/packback-openapi.yml
- filename: packback-openapi.yml
  format: yaml
  label: Packback LTI Integration
  slug: lti-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packback/refs/heads/main/openapi/packback-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: packback.co
  spf: true
hosts:
- cert_expires: Oct  5 04:18:02 2026 GMT
  host: packback.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packback Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packback, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Packback
provider_slug: packback
slug: packback-domain-security
source_filename: packback-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packback.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: packback.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packback/refs/heads/main/security/packback-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- EdTech
- AI
- Discussion
- Writing Feedback
- LTI
- LMS
---
