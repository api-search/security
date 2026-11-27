---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bayt.com
  spf: true
hosts:
- cert_expires: May 29 02:31:42 2027 GMT
  host: bayt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bayt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bayt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bayt
provider_slug: bayt
slug: bayt-domain-security
source_filename: bayt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bayt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 29 02:31:42 2027 GMT\n  hsts: null\ndomains:\n- domain: bayt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bayt/security/bayt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- JobSite
- Middle East
- North-Africa
- Careers
- Recruiting
---
