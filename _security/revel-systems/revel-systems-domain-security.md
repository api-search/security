---
api_specs:
- filename: revel-open-api-openapi.yml
  format: yaml
  label: Revel Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revel-systems/refs/heads/main/openapi/revel-open-api-openapi.yml
- filename: revel-webhooks-asyncapi.yml
  format: yaml
  label: Revel Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/revel-systems/refs/heads/main/asyncapi/revel-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revelsystems.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: revelup.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: revelsystems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 10:44:08 2026 GMT
  host: developer.revelsystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: yoursubdomain.revelup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Revel Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revel Systems, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Revel Systems
provider_slug: revel-systems
slug: revel-systems-domain-security
source_filename: revel-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revelsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\n- host: developer.revelsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:44:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yoursubdomain.revelup.com\n  https: false\ndomains:\n- domain: revelsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: revelup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revel-systems/refs/heads/main/security/revel-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- POS
- Restaurant
- Retail
- iPad
---
