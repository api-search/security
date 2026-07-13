---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bugcrowd.com
  spf: false
hosts:
- cert_expires: Mar 20 03:00:27 2027 GMT
  host: docs.bugcrowd.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bugcrowd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bugcrowd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Bugcrowd
provider_slug: bugcrowd
slug: bugcrowd-domain-security
source_filename: bugcrowd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bugcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 03:00:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: bugcrowd.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bugcrowd/refs/heads/main/security/bugcrowd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Public APIs
---
