---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: socrata.com
  spf: true
hosts:
- cert_expires: Sep 12 19:23:47 2026 GMT
  host: dev.socrata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socrata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socrata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Socrata
provider_slug: socrata
slug: socrata-domain-security
source_filename: socrata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.socrata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socrata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socrata/refs/heads/main/security/socrata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Data
- Public APIs
---
