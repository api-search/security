---
api_specs:
- filename: aeoess-com-openapi-generated.yml
  format: yaml
  label: aeoess API
  slug: aeoess-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aeoess-com/openapi/_ae-authored/aeoess-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aeoess.com
  spf: true
hosts:
- cert_expires: Jan 29 19:32:37 2027 GMT
  host: aeoess.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeoess Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aeoess, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aeoess
provider_slug: aeoess-com
slug: aeoess-com-domain-security
source_filename: aeoess-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aeoess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 19:32:37 2027 GMT\n  hsts: false\ndomains:\n- domain: aeoess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aeoess-com/security/aeoess-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Governance
- Open Source
- AgentAuthority
- Platform
---
