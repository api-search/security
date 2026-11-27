---
api_specs:
- filename: intermind-com-openapi-generated.yml
  format: yaml
  label: InterMIND API
  slug: intermind-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intermind-com/openapi/_ae-authored/intermind-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intermind.com
  spf: true
hosts:
- cert_expires: Jan 29 23:44:44 2027 GMT
  host: intermind.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InterMIND Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InterMIND, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InterMIND
provider_slug: intermind-com
slug: intermind-com-domain-security
source_filename: intermind-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intermind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:44:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: intermind.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/intermind-com/security/intermind-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Multilingual
- Artificial Intelligence
- Real-Time Translation
- Distributed-team
---
