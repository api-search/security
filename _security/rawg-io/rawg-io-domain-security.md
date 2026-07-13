---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rawg.io
  spf: true
hosts:
- cert_expires: Oct  9 08:04:38 2026 GMT
  host: rawg.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rawg Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RAWG.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RAWG.io
provider_slug: rawg-io
slug: rawg-io-domain-security
source_filename: rawg-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rawg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:04:38 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: rawg.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rawg-io/refs/heads/main/security/rawg-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Games And Comics
- Public APIs
---
