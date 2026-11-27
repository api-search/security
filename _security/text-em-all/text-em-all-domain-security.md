---
api_specs:
- filename: text-em-all-openapi-generated.yml
  format: yaml
  label: Call-Em-All, Inc. API
  slug: text-em-all-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-em-all/openapi/_ae-authored/text-em-all-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssltrust.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: text-em-all.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: text-em-all.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Call-Em-All, Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Call-Em-All, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Call-Em-All, Inc.
provider_slug: text-em-all
slug: text-em-all-domain-security
source_filename: text-em-all-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: text-em-all.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: text-em-all.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssltrust.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/text-em-all/security/text-em-all-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- Marketing
- Communications
- Employee-Owned
- Company
---
