---
api_specs:
- filename: iasig-md-openapi-generated.yml
  format: yaml
  label: iAsig API
  slug: iasig-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iasig-md/openapi/_ae-authored/iasig-md-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: iasig.md
  spf: true
hosts:
- cert_expires: Jan 21 12:27:57 2027 GMT
  host: iasig.md
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: iAsig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iAsig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: iAsig
provider_slug: iasig-md
slug: iasig-md-domain-security
source_filename: iasig-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iasig.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 12:27:57 2027 GMT\n  hsts: false\ndomains:\n- domain: iasig.md\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/iasig-md/security/iasig-md-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Moldova
- Comparison
- Online
- iAsig
---
