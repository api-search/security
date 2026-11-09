---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agenty.im
  spf: false
hosts:
- cert_expires: Dec  6 12:01:41 2026 GMT
  host: agenty.im
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agenty Im Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agenty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agenty
provider_slug: agenty-im
slug: agenty-im-domain-security
source_filename: agenty-im-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenty.im\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 12:01:41 2026 GMT\n  hsts: false\ndomains:\n- domain: agenty.im\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agenty-im/security/agenty-im-domain-security.yml
summary_line: TLSv1.3
tags:
- Identity
- Handle verification
- Agent API
---
