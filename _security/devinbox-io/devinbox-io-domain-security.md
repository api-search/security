---
api_specs:
- filename: devinbox-io-openapi-generated.yml
  format: yaml
  label: DevInbox API
  slug: devinbox-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devinbox-io/openapi/_ae-authored/devinbox-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: devinbox.io
  spf: true
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: devinbox.io
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DevInbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevInbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DevInbox
provider_slug: devinbox-io
slug: devinbox-io-domain-security
source_filename: devinbox-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devinbox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: devinbox.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/devinbox-io/security/devinbox-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Email
- Notification
- API Integration
- Shutdown
---
