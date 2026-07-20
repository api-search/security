---
api_specs:
- filename: leeo-insurance-services-fleet-openapi.yml
  format: yaml
  label: LEEO Fleet Telematics API
  slug: leeo-insurance-services-fleet-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeo-insurance-services/refs/heads/main/openapi/leeo-insurance-services-fleet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leeoinsurance.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.leeoinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leeo Insurance Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LEEO Insurance Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LEEO Insurance Services
provider_slug: leeo-insurance-services
slug: leeo-insurance-services-domain-security
source_filename: leeo-insurance-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.leeoinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: leeoinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leeo-insurance-services/refs/heads/main/security/leeo-insurance-services-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Insurtech
- Commercial Auto Insurance
- Telematics
- Fleet Management
- Driving Behavior
- Risk Management
- Managing General Agent
- Mobile SDK
---
