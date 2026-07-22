---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: campusapts.com
  spf: true
hosts:
- cert_expires: Aug 20 10:14:05 2026 GMT
  host: www.campusapts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Campus Apartments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campus Apartments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Campus Apartments
provider_slug: campus-apartments
slug: campus-apartments-domain-security
source_filename: campus-apartments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.campusapts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:14:05 2026 GMT\n  hsts: null\ndomains:\n- domain: campusapts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campus-apartments/refs/heads/main/security/campus-apartments-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Student Housing
- Real Estate
- Property Management
- Higher Education
- Multifamily
- Privately Held
---
