---
api_specs:
- filename: konecranes-openapi-generated.yml
  format: yaml
  label: Konecranes API
  slug: konecranes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/konecranes/openapi/_ae-authored/konecranes-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: konecranes.com
  spf: true
hosts:
- cert_expires: Jan  6 19:25:30 2027 GMT
  host: www.konecranes.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Konecranes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konecranes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Konecranes
provider_slug: konecranes
slug: konecranes-domain-security
source_filename: konecranes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.konecranes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 19:25:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: konecranes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/konecranes/security/konecranes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Material Handling
- Lifting Equipment
- Industrial Solutions
- Global
- Engineering
---
