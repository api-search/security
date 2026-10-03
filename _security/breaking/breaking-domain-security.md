---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: breaking.com
  spf: true
hosts:
- cert_expires: Dec  9 13:36:44 2026 GMT
  host: www.breaking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breaking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breaking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Breaking
provider_slug: breaking
slug: breaking-domain-security
source_filename: breaking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breaking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 13:36:44 2026 GMT\n  hsts: false\ndomains:\n- domain: breaking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breaking/refs/heads/main/security/breaking-domain-security.yml
summary_line: TLSv1.3
tags:
- Plastic Waste
- Chemical Recycling
---
