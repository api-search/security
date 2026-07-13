---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: api.bible
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: docs.api.bible
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Bible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Bible, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Bible
provider_slug: the-bible
slug: the-bible-domain-security
source_filename: the-bible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.api.bible\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: api.bible\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-bible/refs/heads/main/security/the-bible-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Books
- Public APIs
---
