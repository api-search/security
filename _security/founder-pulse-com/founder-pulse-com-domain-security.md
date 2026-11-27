---
api_specs:
- filename: founder-pulse-com-public-api-openapi.yml
  format: yaml
  label: FounderPulse Public API
  slug: founder-pulse-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/founder-pulse-com/openapi/founder-pulse-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: founder-pulse.com
  spf: true
hosts:
- cert_expires: Jan 19 15:55:06 2027 GMT
  host: founder-pulse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FounderPulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FounderPulse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FounderPulse
provider_slug: founder-pulse-com
slug: founder-pulse-com-domain-security
source_filename: founder-pulse-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: founder-pulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 15:55:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: founder-pulse.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/founder-pulse-com/security/founder-pulse-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Business
- Advisor
- Founder Tools
- Software-as-a-Service
---
