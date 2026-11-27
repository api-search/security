---
api_specs:
- filename: letl-ink-openapi-generated.yml
  format: yaml
  label: Letlink API
  slug: letl-ink-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letl-ink/openapi/_ae-authored/letl-ink-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: letl.ink
  spf: true
hosts:
- cert_expires: Feb 10 11:30:26 2027 GMT
  host: letl.ink
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Letlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Letlink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Letlink
provider_slug: letl-ink
slug: letl-ink-domain-security
source_filename: letl-ink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letl.ink\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 11:30:26 2027 GMT\n  hsts: false\ndomains:\n- domain: letl.ink\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/letl-ink/security/letl-ink-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Link Shortener
- Analytics
- Custom Domains
- QR Codes
---
