---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kaman.com
  spf: true
hosts:
- cert_expires: Sep 14 21:09:11 2026 GMT
  host: www.kaman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.kaman.com
  https: false
- host: api.kaman.com
  https: false
kind: domain-security
layout: security
method: probed
name: Kaman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaman Corporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kaman Corporation
provider_slug: kaman
slug: kaman-domain-security
source_filename: kaman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:09:11 2026 GMT\n  hsts: false\n- host: developer.kaman.com\n  https: false\n- host: api.kaman.com\n  https: false\ndomains:\n- domain: kaman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaman/refs/heads/main/security/kaman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Distribution
- Industrial
---
