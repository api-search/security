---
api_specs:
- filename: marrowhealthapp-com-openapi-generated.yml
  format: yaml
  label: Marrow API
  slug: marrowhealthapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marrowhealthapp-com/openapi/_ae-authored/marrowhealthapp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marrowhealthapp.com
  spf: true
hosts:
- cert_expires: Jan  1 14:54:18 2027 GMT
  host: marrowhealthapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marrow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Marrow
provider_slug: marrowhealthapp-com
slug: marrowhealthapp-com-domain-security
source_filename: marrowhealthapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marrowhealthapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 14:54:18 2027 GMT\n  hsts: false\ndomains:\n- domain: marrowhealthapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/marrowhealthapp-com/security/marrowhealthapp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Fitness
- Apple Health
- Artificial Intelligence
- Mobile
---
