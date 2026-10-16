---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crimsoneducation.org
  spf: true
hosts:
- cert_expires: Nov 30 06:02:17 2026 GMT
  host: www.crimsoneducation.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crimson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crimson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crimson
provider_slug: crimson
slug: crimson-domain-security
source_filename: crimson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crimsoneducation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 06:02:17 2026 GMT\n  hsts: null\ndomains:\n- domain: crimsoneducation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crimson/refs/heads/main/security/crimson-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- College Admissions
- Test Preparation
- Consulting
- Global
---
