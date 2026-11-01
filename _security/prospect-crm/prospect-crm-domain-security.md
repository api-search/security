---
api_specs:
- filename: prospect-crm-openapi-generated.yml
  format: yaml
  label: Prospect CRM API
  slug: prospect-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospect-crm/openapi/_ae-authored/prospect-crm-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prospectsoft.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: prospectsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prospect Crm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prospect CRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prospect CRM
provider_slug: prospect-crm
slug: prospect-crm-domain-security
source_filename: prospect-crm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prospectsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: prospectsoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/prospect-crm/security/prospect-crm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
