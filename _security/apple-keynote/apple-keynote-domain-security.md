---
api_specs:
- filename: apple-keynote-icloud-openapi.yaml
  format: yaml
  label: Keynote iCloud API
  slug: keynote-icloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/openapi/apple-keynote-icloud-openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "pki.apple.com"
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
- caa:
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  - 0 iodef "mailto:contact_pki@apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: icloud.com
  spf: true
hosts:
- cert_expires: Aug 27 17:10:52 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 18:07:22 2027 GMT
  host: www.icloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: p00-keynote.icloud.com
  https: false
kind: domain-security
layout: security
method: probed
name: Apple Keynote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apple Keynote, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apple Keynote
provider_slug: apple-keynote
slug: apple-keynote-domain-security
source_filename: apple-keynote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.icloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 18:07:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: p00-keynote.icloud.com\n  https: false\ndomains:\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: icloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/security/apple-keynote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
---
