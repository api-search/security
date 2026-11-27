---
api_specs:
- filename: enablon-openapi-generated.yml
  format: yaml
  label: Enablon API
  slug: enablon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enablon/openapi/_ae-authored/enablon-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: enablon.com
  spf: true
hosts:
- cert_expires: May 14 23:59:59 2027 GMT
  host: www.enablon.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enablon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enablon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Enablon
provider_slug: enablon
slug: enablon-domain-security
source_filename: enablon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enablon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: enablon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/enablon/security/enablon-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- EHS
- Risk Management
- Sustainability
- Compliance
- Enterprise Software
---
