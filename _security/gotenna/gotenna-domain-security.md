---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gotenna.com
  spf: true
hosts:
- cert_expires: Aug 26 18:21:31 2026 GMT
  host: gotenna.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gotenna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoTenna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GoTenna
provider_slug: gotenna
slug: gotenna-domain-security
source_filename: gotenna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gotenna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:21:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: gotenna.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotenna/refs/heads/main/security/gotenna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mesh Networking
- Off-Grid Communication
- Radio
- SDK
- Public Safety
- Defense
- Mobile SDK
- Hardware
---
