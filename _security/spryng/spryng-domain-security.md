---
api_specs:
- filename: spryng-openapi-generated.yml
  format: yaml
  label: Spryng API
  slug: spryng-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spryng/openapi/_ae-authored/spryng-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spryng.nl
  spf: true
hosts:
- cert_expires: Feb  6 17:53:47 2027 GMT
  host: www.spryng.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spryng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spryng, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spryng
provider_slug: spryng
slug: spryng-domain-security
source_filename: spryng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spryng.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 17:53:47 2027 GMT\n  hsts: false\ndomains:\n- domain: spryng.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/spryng/security/spryng-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Messaging
- SMS
- RCS
- WhatsApp Business
- Voice API
---
