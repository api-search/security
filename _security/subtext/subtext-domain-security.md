---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: subtext.com
  spf: false
hosts:
- cert_expires: Jan 27 03:07:07 2027 GMT
  host: subtext.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Subtext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subtext *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Subtext *
provider_slug: subtext
slug: subtext-domain-security
source_filename: subtext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: subtext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 03:07:07 2027 GMT\n  hsts: null\ndomains:\n- domain: subtext.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subtext/refs/heads/main/security/subtext-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Education
- Acquired
---
