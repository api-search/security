---
api_specs:
- filename: gnosari-com-openapi-generated.yml
  format: yaml
  label: Gnosari API
  slug: gnosari-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosari-com/openapi/_ae-authored/gnosari-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gnosari.com
  spf: true
hosts:
- cert_expires: Jan 28 01:31:10 2027 GMT
  host: gnosari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gnosari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gnosari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gnosari
provider_slug: gnosari-com
slug: gnosari-com-domain-security
source_filename: gnosari-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gnosari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 01:31:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gnosari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gnosari-com/security/gnosari-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Conversations
- Surveys
- Data Collection
- Integration
---
