---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mhw-db.com
  spf: false
hosts:
- cert_expires: Sep 17 01:18:18 2026 GMT
  host: docs.mhw-db.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monster Hunter World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monster Hunter World, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Monster Hunter World
provider_slug: monster-hunter-world
slug: monster-hunter-world-domain-security
source_filename: monster-hunter-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mhw-db.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:18:18 2026 GMT\n  hsts: false\ndomains:\n- domain: mhw-db.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monster-hunter-world/refs/heads/main/security/monster-hunter-world-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
