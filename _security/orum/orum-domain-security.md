---
api_specs:
- filename: orum-openapi-original.yml
  format: yaml
  label: Orum API
  slug: orum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: orum.io
  spf: true
hosts:
- cert_expires: Aug 28 03:32:51 2026 GMT
  host: orum.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 03:32:51 2026 GMT
  host: api-sandbox.orum.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: vault.api-sandbox.orum.io
  https: false
kind: domain-security
layout: security
method: probed
name: Orum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orum, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Orum
provider_slug: orum
slug: orum-domain-security
source_filename: orum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:32:51 2026 GMT\n  hsts: null\n- host: api-sandbox.orum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:32:51 2026 GMT\n  hsts: null\n- host: vault.api-sandbox.orum.io\n  https: false\ndomains:\n- domain: orum.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/security/orum-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Payments
- Fintech
- Banking
- Instant Payments
- ACH
- Money Movement
- Bank Account Verification
---
