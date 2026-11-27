---
api_specs:
- filename: usethisskill-com-openapi-generated.yml
  format: yaml
  label: Use This Skill API
  slug: usethisskill-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usethisskill-com/openapi/_ae-authored/usethisskill-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usethisskill.com
  spf: true
hosts:
- cert_expires: Feb 16 17:08:13 2027 GMT
  host: usethisskill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Use This Skill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Use This Skill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Use This Skill
provider_slug: usethisskill-com
slug: usethisskill-com-domain-security
source_filename: usethisskill-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usethisskill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 17:08:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usethisskill.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usethisskill-com/security/usethisskill-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Development
- Skills
- Platform
- Community
---
