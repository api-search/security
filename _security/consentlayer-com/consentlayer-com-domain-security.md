---
api_specs:
- filename: consentlayer-com-openapi-generated.yml
  format: yaml
  label: ConsentLayer API
  slug: consentlayer-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consentlayer-com/openapi/_ae-authored/consentlayer-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: consentlayer.com
  spf: true
hosts:
- cert_expires: Dec 26 16:47:05 2026 GMT
  host: consentlayer.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ConsentLayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConsentLayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ConsentLayer
provider_slug: consentlayer-com
slug: consentlayer-com-domain-security
source_filename: consentlayer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: consentlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:47:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: consentlayer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/consentlayer-com/security/consentlayer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cookie Consent
- AI Integration
- Tracker Blocking
- Privacy Compliance
- Consent Logging
---
