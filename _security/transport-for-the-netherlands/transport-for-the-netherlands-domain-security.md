---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ns.nl
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: www.ns.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For The Netherlands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for The Netherlands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Transport for The Netherlands
provider_slug: transport-for-the-netherlands
slug: transport-for-the-netherlands-domain-security
source_filename: transport-for-the-netherlands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ns.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ns.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-the-netherlands/refs/heads/main/security/transport-for-the-netherlands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
