---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: redventures.com
  spf: true
hosts:
- cert_expires: Sep  8 08:13:16 2026 GMT
  host: www.redventures.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Red Ventures
provider_slug: red-ventures
slug: red-ventures-domain-security
source_filename: red-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redventures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 08:13:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: redventures.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-ventures/refs/heads/main/security/red-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Marketing
- Digital Marketing
- Portfolio
- Holding Company
---
