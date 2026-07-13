---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: substack.com
  spf: true
hosts:
- cert_expires: Aug 22 07:50:09 2026 GMT
  host: substack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:44:59 2026 GMT
  host: support.substack.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Substack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Substack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Substack
provider_slug: substack
slug: substack-domain-security
source_filename: substack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: substack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:50:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.substack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: substack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/substack/refs/heads/main/security/substack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Newsletters
- Publishing
- Creator Economy
- Subscriptions
- Email
- Podcasting
- Notes
- Media
- Independent Media
- Paid Content
---
