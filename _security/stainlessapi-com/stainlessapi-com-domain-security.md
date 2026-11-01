---
api_specs:
- filename: stainlessapi-com-openapi-generated.yml
  format: yaml
  label: Stainless API
  slug: stainlessapi-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stainlessapi-com/openapi/_ae-authored/stainlessapi-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stainlessapi.com
  spf: true
hosts:
- host: www.stainlessapi.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stainlessapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stainless, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stainless
provider_slug: stainlessapi-com
slug: stainlessapi-com-domain-security
source_filename: stainlessapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stainlessapi.com\n  https: false\ndomains:\n- domain: stainlessapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/stainlessapi-com/security/stainlessapi-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
