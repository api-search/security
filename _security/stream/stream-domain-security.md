---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:abuse-caa@firma.seznam.cz"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stream.cz
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.stream.cz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stream
provider_slug: stream
slug: stream-domain-security
source_filename: stream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.stream.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stream.cz\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:abuse-caa@firma.seznam.cz\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream/refs/heads/main/security/stream-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Video
- Public APIs
---
