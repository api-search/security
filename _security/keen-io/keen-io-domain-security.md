---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keen.io
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: keen.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keen Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keen IO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keen IO
provider_slug: keen-io
slug: keen-io-domain-security
source_filename: keen-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: keen.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keen-io/refs/heads/main/security/keen-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Machine Learning
- Public APIs
---
