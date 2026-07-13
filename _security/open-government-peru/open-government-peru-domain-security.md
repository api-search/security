---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.pe
  spf: false
hosts:
- cert_expires: Sep  6 19:00:58 2026 GMT
  host: www.datosabiertos.gob.pe
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Peru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Peru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Open Government, Peru
provider_slug: open-government-peru
slug: open-government-peru-domain-security
source_filename: open-government-peru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datosabiertos.gob.pe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:00:58 2026 GMT\n  hsts: null\ndomains:\n- domain: gob.pe\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-peru/refs/heads/main/security/open-government-peru-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Government
- Public APIs
---
