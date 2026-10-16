---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: compassjapan.com
  spf: true
hosts:
- cert_expires: Dec 26 04:10:59 2026 GMT
  host: www.compassjapan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compassjapan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compassjapan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Compassjapan
provider_slug: compassjapan
slug: compassjapan-domain-security
source_filename: compassjapan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.compassjapan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 04:10:59 2026 GMT\n  hsts: false\ndomains:\n- domain: compassjapan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compassjapan/refs/heads/main/security/compassjapan-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Export
- Forklift
- Vehicles
- Industrial
---
