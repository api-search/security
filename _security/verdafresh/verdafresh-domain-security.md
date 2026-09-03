---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: verdafresh.com
  spf: true
hosts:
- cert_expires: Oct  5 00:53:47 2026 GMT
  host: verdafresh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdafresh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VerdaFresh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: VerdaFresh
provider_slug: verdafresh
slug: verdafresh-domain-security
source_filename: verdafresh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verdafresh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verdafresh.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdafresh/refs/heads/main/security/verdafresh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Packaging
- Flexible Packaging
- Food Packaging
- Materials Science
- Barrier Coatings
- Recycling
- Sustainability
- Circular Economy
- Manufacturing
---
