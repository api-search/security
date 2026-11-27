---
api_specs:
- filename: temp-mail-io-openapi-generated.yml
  format: yaml
  label: Temp Mail API
  slug: temp-mail-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temp-mail-io/openapi/_ae-authored/temp-mail-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: temp-mail.io
  spf: true
hosts:
- cert_expires: Feb 14 23:46:00 2027 GMT
  host: temp-mail.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Temp Mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temp Mail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temp Mail
provider_slug: temp-mail-io
slug: temp-mail-io-domain-security
source_filename: temp-mail-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temp-mail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:46:00 2027 GMT\n  hsts: false\ndomains:\n- domain: temp-mail.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/temp-mail-io/security/temp-mail-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Disposable
- Privacy
- API
---
