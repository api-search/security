---
api_specs:
- filename: deyaho-com-openapi-generated.yml
  format: yaml
  label: Deyaho API
  slug: deyaho-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deyaho-com/openapi/_ae-authored/deyaho-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deyaho.com
  spf: true
hosts:
- cert_expires: Dec 15 17:50:37 2026 GMT
  host: deyaho.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deyaho Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deyaho, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deyaho
provider_slug: deyaho-com
slug: deyaho-com-domain-security
source_filename: deyaho-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deyaho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 17:50:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deyaho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/deyaho-com/security/deyaho-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Voice
- Text
- Multilingual
- Automation
- Company
---
