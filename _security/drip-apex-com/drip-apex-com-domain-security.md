---
api_specs:
- filename: drip-apex-com-openapi-generated.yml
  format: yaml
  label: DRIP Apex API
  slug: drip-apex-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drip-apex-com/openapi/_ae-authored/drip-apex-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drip-apex.com
  spf: true
hosts:
- cert_expires: Jan 13 15:39:18 2027 GMT
  host: drip-apex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DRIP Apex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DRIP Apex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DRIP Apex
provider_slug: drip-apex-com
slug: drip-apex-com-domain-security
source_filename: drip-apex-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drip-apex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:39:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: drip-apex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/drip-apex-com/security/drip-apex-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- A/B Testing
- Artificial Intelligence
- Marketing
- Feature Flags
- Personalization
---
