---
api_specs:
- filename: dataify-com-openapi-generated.yml
  format: yaml
  label: Dataify API
  slug: dataify-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataify-com/openapi/_ae-authored/dataify-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dataify.com
  spf: true
hosts:
- cert_expires: Mar 13 06:51:21 2027 GMT
  host: dataify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dataify
provider_slug: dataify-com
slug: dataify-com-domain-security
source_filename: dataify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 06:51:21 2027 GMT\n  hsts: null\ndomains:\n- domain: dataify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dataify-com/security/dataify-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Data
- Platform
- Real-Time
- Enterprise
- Company
---
