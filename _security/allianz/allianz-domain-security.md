---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz.com
  spf: true
hosts:
- cert_expires: Aug 12 16:58:20 2026 GMT
  host: www.allianz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allianz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allianz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allianz
provider_slug: allianz
slug: allianz-domain-security
source_filename: allianz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allianz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz/refs/heads/main/security/allianz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Financial
- Asset Management
---
