---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zipsec.com
  spf: true
hosts:
- cert_expires: Oct 12 14:18:02 2026 GMT
  host: www.zipsec.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zip Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zip Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zip Security
provider_slug: zip-security
slug: zip-security-domain-security
source_filename: zip-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zipsec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zipsec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zip-security/refs/heads/main/security/zip-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Compliance
- Endpoint Security
- Device Management
- Identity
- MDM
- Managed Security
---
