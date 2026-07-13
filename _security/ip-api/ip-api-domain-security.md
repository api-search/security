---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ip-api.com
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: ip-api.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ip Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ip-api, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ip-api
provider_slug: ip-api
slug: ip-api-domain-security
source_filename: ip-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ip-api.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ip-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ip-api/refs/heads/main/security/ip-api-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Geocoding
- Public APIs
---
