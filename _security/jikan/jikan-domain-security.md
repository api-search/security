---
description: ''
domains:
- caa:
  - hardcore-archimedes-6ebd1f.netlify.com.
  dmarc: false
  dnssec: true
  domain: jikan.moe
  spf: true
hosts:
- cert_expires: Jul 26 11:03:44 2026 GMT
  host: jikan.moe
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jikan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jikan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Jikan
provider_slug: jikan
slug: jikan-domain-security
source_filename: jikan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jikan.moe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 11:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jikan.moe\n  dnssec: true\n  caa:\n  - hardcore-archimedes-6ebd1f.netlify.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jikan/refs/heads/main/security/jikan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Anime
- Public APIs
---
