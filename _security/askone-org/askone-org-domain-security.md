---
api_specs:
- filename: askone-org-openapi-generated.yml
  format: yaml
  label: AskOne API
  slug: askone-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askone-org/openapi/_ae-authored/askone-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: askone.org
  spf: false
hosts:
- cert_expires: Dec  3 16:46:50 2026 GMT
  host: askone.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AskOne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AskOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AskOne
provider_slug: askone-org
slug: askone-org-domain-security
source_filename: askone-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askone.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:46:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: askone.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/askone-org/security/askone-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Moderation
- LiveQ&A
- Audience Engagement
- WebinarTools
- FreePlatform
---
