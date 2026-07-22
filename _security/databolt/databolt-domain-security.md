---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: databolt.io
  spf: true
hosts:
- cert_expires: Sep  6 23:01:50 2026 GMT
  host: www.databolt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Databolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databolt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Databolt
provider_slug: databolt
slug: databolt-domain-security
source_filename: databolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.databolt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:01:50 2026 GMT\n  hsts: false\ndomains:\n- domain: databolt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databolt/refs/heads/main/security/databolt-domain-security.yml
summary_line: TLSv1.3
tags:
- Agency
- Custom Applications
- Data Processing
- Digital Design
- SEO
- UI/UX
- Web Development
- WordPress
---
