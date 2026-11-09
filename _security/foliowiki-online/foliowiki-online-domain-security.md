---
api_specs:
- filename: foliowiki-online-openapi-generated.yml
  format: yaml
  label: Folio API
  slug: foliowiki-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foliowiki-online/openapi/_ae-authored/foliowiki-online-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foliowiki.online
  spf: false
hosts:
- cert_expires: Jan  3 16:15:00 2027 GMT
  host: foliowiki.online
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foliowiki Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Folio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Folio
provider_slug: foliowiki-online
slug: foliowiki-online-domain-security
source_filename: foliowiki-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foliowiki.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 16:15:00 2027 GMT\n  hsts: false\ndomains:\n- domain: foliowiki.online\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/foliowiki-online/security/foliowiki-online-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Wiki
- Documentation
- Open Source
- Self‑hosted
- Git‑based
- Collaboration
- AI Assistant
- Docs as Code
---
