---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orangelogic.com
  spf: true
hosts:
- cert_expires: Sep 21 17:48:48 2026 GMT
  host: www.orangelogic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:13:57 2026 GMT
  host: developer.orangelogic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orangelogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orange Logic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orange Logic
provider_slug: orangelogic
slug: orangelogic-domain-security
source_filename: orangelogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orangelogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 17:48:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.orangelogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orangelogic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orangelogic/refs/heads/main/security/orangelogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- DAM
- Media Asset Management
- MAM
- Enterprise
- Metadata
- Archive
---
