---
api_specs:
- filename: featurejet-com-openapi-generated.yml
  format: yaml
  label: FeatureJet API
  slug: featurejet-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/featurejet-com/openapi/_ae-authored/featurejet-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: featurejet.com
  spf: true
hosts:
- cert_expires: Feb  4 10:27:54 2027 GMT
  host: featurejet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FeatureJet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FeatureJet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FeatureJet
provider_slug: featurejet-com
slug: featurejet-com-domain-security
source_filename: featurejet-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: featurejet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 10:27:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: featurejet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/featurejet-com/security/featurejet-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Feedback board
- AI Agents
- Roadmaps
- Software-as-a-Service
---
