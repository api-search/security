---
api_specs:
- filename: appendix-com-api-reference-openapi-generated.yml
  format: yaml
  label: Appendix api reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appendix-com/openapi/_ae-authored/appendix-com-api-reference-openapi-generated.yml
- filename: appendix-com-core-openapi-generated.yml
  format: yaml
  label: Appendix core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appendix-com/openapi/_ae-authored/appendix-com-core-openapi-generated.yml
- filename: appendix-com-prescribing-openapi-generated.yml
  format: yaml
  label: Appendix Prescribing API Overview API
  slug: prescribing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appendix-com/openapi/_ae-authored/appendix-com-prescribing-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appendix.com
  spf: true
hosts:
- cert_expires: Dec 26 15:45:58 2026 GMT
  host: appendix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appendix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appendix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appendix
provider_slug: appendix-com
slug: appendix-com-domain-security
source_filename: appendix-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:45:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: appendix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/appendix-com/security/appendix-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Artificial Intelligence
- Telehealth
- PhysicianReview
---
