---
api_specs:
- filename: alterauth-com-openapi-generated.yml
  format: yaml
  label: Alter API
  slug: alterauth-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alterauth-com/openapi/_ae-authored/alterauth-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alterauth.com
  spf: true
hosts:
- cert_expires: Jan  5 01:31:02 2027 GMT
  host: alterauth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alterauth Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alter
provider_slug: alterauth-com
slug: alterauth-com-domain-security
source_filename: alterauth-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alterauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 01:31:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alterauth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/alterauth-com/security/alterauth-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Artificial Intelligence
- Privileged Access Management
- Identity and Access Management
- Privileged
---
