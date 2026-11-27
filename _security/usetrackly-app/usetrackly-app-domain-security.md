---
api_specs:
- filename: usetrackly-app-companies-api-openapi.yml
  format: yaml
  label: Trackly Companies API
  slug: usetrackly-app-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetrackly-app/openapi/usetrackly-app-companies-api-openapi.yml
- filename: usetrackly-app-jobs-api-openapi.yml
  format: yaml
  label: Trackly Jobs API
  slug: usetrackly-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetrackly-app/openapi/usetrackly-app-jobs-api-openapi.yml
- filename: usetrackly-app-user-api-openapi.yml
  format: yaml
  label: Trackly User API
  slug: usetrackly-app-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetrackly-app/openapi/usetrackly-app-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usetrackly.app
  spf: true
hosts:
- cert_expires: Feb 18 03:28:59 2027 GMT
  host: usetrackly.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trackly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trackly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trackly
provider_slug: usetrackly-app
slug: usetrackly-app-domain-security
source_filename: usetrackly-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usetrackly.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 03:28:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usetrackly.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usetrackly-app/security/usetrackly-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job Search
- Student Recruiting
- AI Agent
- Career Page Monitoring
---
