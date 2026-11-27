---
api_specs:
- filename: enhanced-radar-openapi-generated.yml
  format: yaml
  label: Enhanced Radar API
  slug: enhanced-radar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enhanced-radar/openapi/_ae-authored/enhanced-radar-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enhancedradar.com
  spf: true
hosts:
- cert_expires: May 15 23:59:59 2027 GMT
  host: www.enhancedradar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: May 15 23:59:59 2027 GMT
  host: enhancedradar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: May  2 23:59:59 2027 GMT
  host: api.enhancedradar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Enhanced Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enhanced Radar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enhanced Radar
provider_slug: enhanced-radar
slug: enhanced-radar-domain-security
source_filename: enhanced-radar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enhancedradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 15 23:59:59 2027 GMT\n  hsts: false\n- host: enhancedradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 15 23:59:59 2027 GMT\n  hsts: false\n- host: api.enhancedradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: enhancedradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/enhanced-radar/security/enhanced-radar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aviation
- Artificial Intelligence
- Air Traffic Control
- Aviation Safety
- Machine Learning
- Datasets
- Transportation
---
