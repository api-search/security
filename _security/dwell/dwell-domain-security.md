---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dwell.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: dwell.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dwell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: dwell
provider_slug: dwell
slug: dwell-domain-security
source_filename: dwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dwell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwell/refs/heads/main/security/dwell-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Media
- Publishing
- Home Design
- Architecture
- Interior Design
- Real Estate
---
