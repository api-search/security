---
api_specs:
- filename: omniaauto-ca-openapi.json
  format: json
  label: OmniaAuto API
  slug: omniaauto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniaauto-ca/openapi/omniaauto-ca-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: omniaauto.ca
  spf: true
hosts:
- cert_expires: Dec 19 03:11:43 2026 GMT
  host: omniaauto.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Omniaauto Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for omniaauto-ca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: omniaauto-ca
provider_slug: omniaauto-ca
slug: omniaauto-ca-domain-security
source_filename: omniaauto-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omniaauto.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 03:11:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: omniaauto.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/omniaauto-ca/security/omniaauto-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Data
- API
- Market
---
