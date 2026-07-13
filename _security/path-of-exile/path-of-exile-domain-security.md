---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pathofexile.com
  spf: true
hosts:
- cert_expires: Aug 14 03:00:14 2026 GMT
  host: www.pathofexile.com
  hsts: true
  hsts_max_age: 63115200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Path Of Exile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Path of Exile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Path of Exile
provider_slug: path-of-exile
slug: path-of-exile-domain-security
source_filename: path-of-exile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pathofexile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63115200\ndomains:\n- domain: pathofexile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/path-of-exile/refs/heads/main/security/path-of-exile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Public APIs
---
