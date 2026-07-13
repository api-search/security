---
api_specs:
- filename: api
  format: yaml
  label: Userflow REST API
  slug: userflow-rest-api
  spec_type: OpenAPI
  url: https://docs.userflow.com/docs/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: userflow.com
  spf: true
hosts:
- cert_expires: Sep 10 18:10:33 2026 GMT
  host: www.userflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:28:53 2026 GMT
  host: docs.userflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:28:59 2026 GMT
  host: api.userflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Userflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Userflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Userflow
provider_slug: userflow
slug: userflow-domain-security
source_filename: userflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.userflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:10:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.userflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.userflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:28:59 2026 GMT\n  hsts: null\ndomains:\n- domain: userflow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userflow/refs/heads/main/security/userflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- User Onboarding
- Product Adoption
- In-App Guides
- Checklists
- Announcements
- NPS Surveys
- User Flows
- SaaS
- Product-Led Growth
---
