---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lockheedmartin.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.lockheedmartin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lockheed Martin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lockheed Martin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lockheed Martin
provider_slug: lockheed-martin
slug: lockheed-martin-domain-security
source_filename: lockheed-martin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lockheedmartin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lockheedmartin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lockheed-martin/refs/heads/main/security/lockheed-martin-domain-security.yml
summary_line: TLSv1.3
tags:
- Defense
- Aerospace
- Security
- Fortune 500
---
