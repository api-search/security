---
api_specs:
- filename: lead-radar-fr-api-openapi.json
  format: json
  label: Lead Radar API API
  slug: lead-radar-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lead-radar-fr/openapi/_original/lead-radar-fr-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lead-radar.fr
  spf: true
hosts:
- cert_expires: Jan 17 08:52:59 2027 GMT
  host: lead-radar.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lead Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lead Radar
provider_slug: lead-radar-fr
slug: lead-radar-fr-domain-security
source_filename: lead-radar-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lead-radar.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 08:52:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lead-radar.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lead-radar-fr/security/lead-radar-fr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- B2B
- Lead Generation
- French Market
- Software-as-a-Service
- Prospecting
---
