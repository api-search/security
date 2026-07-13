---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jokes.one
  spf: true
hosts:
- cert_expires: Sep 23 18:35:26 2026 GMT
  host: jokes.one
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jokes One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jokes One, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jokes One
provider_slug: jokes-one
slug: jokes-one-domain-security
source_filename: jokes-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jokes.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:35:26 2026 GMT\n  hsts: false\ndomains:\n- domain: jokes.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jokes-one/refs/heads/main/security/jokes-one-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
