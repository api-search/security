---
api_specs:
- filename: erechio-pr-fen-api-openapi.yml
  format: yaml
  label: Erechio Prüfen API
  slug: erechio-pr-fen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/erechio/openapi/erechio-pr-fen-api-openapi.yml
- filename: erechio-status-api-openapi.yml
  format: yaml
  label: Erechio Status API
  slug: erechio-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/erechio/openapi/erechio-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: erechio.de
  spf: true
hosts:
- cert_expires: Jan 13 09:03:28 2027 GMT
  host: erechio.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Erechio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erechio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Erechio
provider_slug: erechio
slug: erechio-domain-security
source_filename: erechio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erechio.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 09:03:28 2027 GMT\n  hsts: false\ndomains:\n- domain: erechio.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/erechio/security/erechio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- German
- e-invoice
- Validation
- XRechnung
- ZUGFeRD
- KoSIT
---
