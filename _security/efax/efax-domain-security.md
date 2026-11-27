---
api_specs:
- filename: efax-openapi-generated.yml
  format: yaml
  label: eFax API
  slug: efax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/efax/openapi/_ae-authored/efax-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: efax.com
  spf: true
hosts:
- cert_expires: Jan 30 06:17:13 2027 GMT
  host: efax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eFax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eFax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eFax
provider_slug: efax
slug: efax-domain-security
source_filename: efax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: efax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 06:17:13 2027 GMT\n  hsts: null\ndomains:\n- domain: efax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/efax/security/efax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fax
- Cloud Fax
- Healthcare
- Government
- Managed Service
- Enterprise
---
