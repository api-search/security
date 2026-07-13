---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipapi.co
  spf: true
hosts:
- cert_expires: Sep 13 06:11:34 2026 GMT
  host: ipapi.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ipapi Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ipapi.co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ipapi.co
provider_slug: ipapi-co
slug: ipapi-co-domain-security
source_filename: ipapi-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipapi.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 06:11:34 2026 GMT\n  hsts: false\ndomains:\n- domain: ipapi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipapi-co/refs/heads/main/security/ipapi-co-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Geocoding
- Public APIs
---
