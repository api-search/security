---
api_specs:
- filename: terlido-com-openapi-generated.yml
  format: yaml
  label: Terlido API
  slug: terlido-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terlido-com/openapi/_ae-authored/terlido-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: terlido.com
  spf: true
hosts:
- cert_expires: Feb  7 05:55:23 2027 GMT
  host: terlido.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Terlido Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terlido, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Terlido
provider_slug: terlido-com
slug: terlido-com-domain-security
source_filename: terlido-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terlido.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 05:55:23 2027 GMT\n  hsts: false\ndomains:\n- domain: terlido.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/terlido-com/security/terlido-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Newsletter
- Cold-Email
- AI
---
