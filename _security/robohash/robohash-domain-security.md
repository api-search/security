---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: robohash.org
  spf: true
hosts:
- cert_expires: Aug 30 22:58:35 2026 GMT
  host: robohash.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robohash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RoboHash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RoboHash
provider_slug: robohash
slug: robohash-domain-security
source_filename: robohash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robohash.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 22:58:35 2026 GMT\n  hsts: null\ndomains:\n- domain: robohash.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robohash/refs/heads/main/security/robohash-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Test Data
- Public APIs
---
