---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: count.ly
  spf: true
hosts:
- cert_expires: Oct  2 16:11:05 2026 GMT
  host: api.count.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Countly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Countly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Countly
provider_slug: countly
slug: countly-domain-security
source_filename: countly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.count.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:11:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: count.ly\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countly/refs/heads/main/security/countly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Source Projects
- Public APIs
---
