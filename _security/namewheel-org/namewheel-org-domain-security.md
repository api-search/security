---
api_specs:
- filename: namewheel-org-openapi-generated.yml
  format: yaml
  label: NameWheel API
  slug: namewheel-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namewheel-org/openapi/_ae-authored/namewheel-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: namewheel.org
  spf: true
hosts:
- cert_expires: Dec 25 17:24:50 2026 GMT
  host: namewheel.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NameWheel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NameWheel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NameWheel
provider_slug: namewheel-org
slug: namewheel-org-domain-security
source_filename: namewheel-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namewheel.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 17:24:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: namewheel.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/namewheel-org/security/namewheel-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tools
- Education
- Free
- Privacy
---
