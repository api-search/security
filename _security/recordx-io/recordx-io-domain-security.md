---
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@recordx.io"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: true
  domain: recordx.io
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: recordx.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RecordX Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RecordX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: RecordX
provider_slug: recordx-io
slug: recordx-io-domain-security
source_filename: recordx-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recordx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: recordx.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:abuse@recordx.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/recordx-io/security/recordx-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Meeting
- Transcription
- Productivity
- SaaS
---
