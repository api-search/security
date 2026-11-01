---
api_specs:
- filename: flashduty-openapi-generated.yml
  format: yaml
  label: Flashduty API
  slug: flashduty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashduty/openapi/_ae-authored/flashduty-openapi-generated.yml
description: ''
domains:
- caa:
  - 32fc6d90dbd9116e.vercel-dns-017.com.
  - 0 issue "sectigo.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: true
  domain: flashduty.com
  spf: false
hosts:
- cert_expires: Dec 22 21:22:22 2026 GMT
  host: flashduty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flashduty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flashduty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Flashduty
provider_slug: flashduty
slug: flashduty-domain-security
source_filename: flashduty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flashduty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:22:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flashduty.com\n  dnssec: true\n  caa:\n  - 32fc6d90dbd9116e.vercel-dns-017.com.\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flashduty/security/flashduty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Incident Response
- AI
- Monitoring
- On-call
- Observability
- Company
---
