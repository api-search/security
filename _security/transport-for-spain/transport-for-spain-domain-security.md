---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: renfe.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: data.renfe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Spain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Spain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transport for Spain
provider_slug: transport-for-spain
slug: transport-for-spain-domain-security
source_filename: transport-for-spain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.renfe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: renfe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-spain/refs/heads/main/security/transport-for-spain-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
