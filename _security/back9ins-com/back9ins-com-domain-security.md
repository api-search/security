---
api_specs:
- filename: back9ins-com-openapi-generated.yml
  format: yaml
  label: back9ins-com API
  slug: back9ins-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/back9ins-com/openapi/_ae-authored/back9ins-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: back9ins.com
  spf: true
hosts:
- cert_expires: Dec 29 14:46:00 2026 GMT
  host: back9ins.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Back9Ins Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for back9ins-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: back9ins-com
provider_slug: back9ins-com
slug: back9ins-com-domain-security
source_filename: back9ins-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: back9ins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 14:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: back9ins.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/back9ins-com/security/back9ins-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- InsurTech
- SaaS
- B2B
- LifeInsurance
---
