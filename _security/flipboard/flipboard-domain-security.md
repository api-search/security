---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flipboard.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: flipboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  7 17:24:42 2026 GMT
  host: about.flipboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flipboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipboard, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flipboard
provider_slug: flipboard
slug: flipboard-domain-security
source_filename: flipboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flipboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: about.flipboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 17:24:42 2026 GMT\n  hsts: false\ndomains:\n- domain: flipboard.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipboard/refs/heads/main/security/flipboard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ActivityPub
- Content Curation
- Digital Publishing
- Fediverse
- News
- RSS
- Social Media
---
