---
api_specs:
- filename: franklymail-com-openapi-generated.yml
  format: yaml
  label: FranklyMail API
  slug: franklymail-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/franklymail-com/openapi/_ae-authored/franklymail-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: franklymail.com
  spf: true
hosts:
- cert_expires: Jan  8 13:54:07 2027 GMT
  host: franklymail.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FranklyMail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FranklyMail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FranklyMail
provider_slug: franklymail-com
slug: franklymail-com-domain-security
source_filename: franklymail-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: franklymail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 13:54:07 2027 GMT\n  hsts: false\ndomains:\n- domain: franklymail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/franklymail-com/security/franklymail-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Collaboration
- Software-as-a-Service
- Small Business
- Privacy
---
