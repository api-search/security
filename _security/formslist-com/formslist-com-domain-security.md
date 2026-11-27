---
api_specs:
- filename: formslist-com-openapi.yml
  format: yaml
  label: FormsList API
  slug: formslist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formslist-com/openapi/formslist-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formslist.com
  spf: true
hosts:
- cert_expires: Dec 17 18:17:43 2026 GMT
  host: formslist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FormsList Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FormsList, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FormsList
provider_slug: formslist-com
slug: formslist-com-domain-security
source_filename: formslist-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formslist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 18:17:43 2026 GMT\n  hsts: false\ndomains:\n- domain: formslist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/formslist-com/security/formslist-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Form Backend
- Developer Tools
- Spam Protection
- Integration
- Software-as-a-Service
---
