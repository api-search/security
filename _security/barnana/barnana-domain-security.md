---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: barnana.com
  spf: true
hosts:
- cert_expires: Dec 26 00:01:35 2026 GMT
  host: barnana.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Barnana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barnana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Barnana
provider_slug: barnana
slug: barnana-domain-security
source_filename: barnana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barnana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 00:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: barnana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barnana/refs/heads/main/security/barnana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SnackFood
- Sustainable
- Organic
- Plant-Based
- Retail
---
