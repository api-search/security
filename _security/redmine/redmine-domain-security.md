---
api_specs:
- filename: redmine-openapi.yml
  format: yaml
  label: Redmine REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: redmine.org
  spf: true
hosts:
- cert_expires: Aug 12 03:03:32 2026 GMT
  host: www.redmine.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redmine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redmine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Redmine
provider_slug: redmine
slug: redmine-domain-security
source_filename: redmine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redmine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 03:03:32 2026 GMT\n  hsts: false\ndomains:\n- domain: redmine.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/security/redmine-domain-security.yml
summary_line: TLSv1.3
tags:
- Project Management
- Issue Tracking
- Open Source
- Ruby on Rails
- Bug Tracking
- Time Tracking
---
