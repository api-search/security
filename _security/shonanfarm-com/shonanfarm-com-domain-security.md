---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shonanfarm.com
  spf: true
hosts:
- cert_expires: Jan 19 00:18:49 2027 GMT
  host: shonanfarm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shonanfarm Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shonanfarm-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: shonanfarm-com
provider_slug: shonanfarm-com
slug: shonanfarm-com-domain-security
source_filename: shonanfarm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shonanfarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 00:18:49 2027 GMT\n  hsts: false\ndomains:\n- domain: shonanfarm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/shonanfarm-com/security/shonanfarm-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Stub
- Unknown
- API
- Placeholder
---
