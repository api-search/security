---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smashfly.com
  spf: true
hosts:
- cert_expires: Oct  8 15:12:23 2026 GMT
  host: www.smashfly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Smashfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smashfly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Smashfly
provider_slug: smashfly
slug: smashfly-domain-security
source_filename: smashfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smashfly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 15:12:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smashfly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smashfly/refs/heads/main/security/smashfly-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Recruitment Marketing
- Talent Acquisition
- HR Technology
- Recruiting CRM
- Programmatic Job Advertising
- Career Sites
---
