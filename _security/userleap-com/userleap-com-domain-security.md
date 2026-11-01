---
api_specs:
- filename: userleap-com-openapi-generated.yml
  format: yaml
  label: Sprig API
  slug: userleap-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userleap-com/openapi/_ae-authored/userleap-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: userleap.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: userleap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Userleap Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sprig
provider_slug: userleap-com
slug: userleap-com-domain-security
source_filename: userleap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: userleap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/userleap-com/security/userleap-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Survey
- Enterprise Research
- AI Agents
- Market Insights
- Customer Experience
- Prototype Testing
- Omnichannel Distribution
---
