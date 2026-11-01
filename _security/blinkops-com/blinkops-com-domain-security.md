---
api_specs:
- filename: blinkops-com-openapi-generated.yml
  format: yaml
  label: Blink API
  slug: blinkops-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkops-com/openapi/_ae-authored/blinkops-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blinkops.com
  spf: true
hosts:
- cert_expires: Dec 13 17:18:32 2026 GMT
  host: blinkops.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blinkops Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blink
provider_slug: blinkops-com
slug: blinkops-com-domain-security
source_filename: blinkops-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 17:18:32 2026 GMT\n  hsts: null\ndomains:\n- domain: blinkops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/blinkops-com/security/blinkops-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
