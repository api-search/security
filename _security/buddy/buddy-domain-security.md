---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "geotrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buddy.works
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: buddy.works
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buddy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Buddy
provider_slug: buddy
slug: buddy-domain-security
source_filename: buddy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buddy.works\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buddy.works\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buddy/refs/heads/main/security/buddy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Continuous Integration
- Public APIs
---
