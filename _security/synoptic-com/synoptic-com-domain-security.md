---
api_specs:
- filename: synoptic-com-asyncapi.yaml
  format: yaml
  label: Synoptic AsyncAPI
  slug: synoptic-asyncapi
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/synoptic-com/asyncapi/synoptic-com-asyncapi.yaml
- filename: synoptic-com-openapi-generated.yml
  format: yaml
  label: Synoptic API
  slug: synoptic-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synoptic-com/openapi/_ae-authored/synoptic-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synoptic.com
  spf: true
hosts:
- cert_expires: May  8 23:59:59 2027 GMT
  host: synoptic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synoptic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synoptic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synoptic
provider_slug: synoptic-com
slug: synoptic-com-domain-security
source_filename: synoptic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synoptic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synoptic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synoptic-com/security/synoptic-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Real-time
- Finance
- News
- API
---
