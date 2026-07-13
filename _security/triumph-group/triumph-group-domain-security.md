---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: triumphgroup.com
  spf: true
- caa:
  - triumphsupplysource.com.cdn.cloudflare.net.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: triumphsupplysource.com
  spf: true
hosts:
- cert_expires: Oct  9 04:58:21 2026 GMT
  host: www.triumphgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 01:54:39 2026 GMT
  host: triumphsupplysource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: dev.triumphgroup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Triumph Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triumph Group, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Triumph Group
provider_slug: triumph-group
slug: triumph-group-domain-security
source_filename: triumph-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.triumphgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:58:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: triumphsupplysource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 01:54:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.triumphgroup.com\n  https: false\ndomains:\n- domain: triumphgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: triumphsupplysource.com\n  dnssec: true\n  caa:\n  - triumphsupplysource.com.cdn.cloudflare.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triumph-group/refs/heads/main/security/triumph-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aerospace
- Defense
- Manufacturing
- Maintenance Repair Overhaul
- Aviation
- Fortune 1000
---
