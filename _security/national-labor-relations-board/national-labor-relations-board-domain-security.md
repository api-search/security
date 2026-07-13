---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nlrb.gov
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.nlrb.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: National Labor Relations Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Labor Relations Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Labor Relations Board
provider_slug: national-labor-relations-board
slug: national-labor-relations-board-domain-security
source_filename: national-labor-relations-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nlrb.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nlrb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-labor-relations-board/refs/heads/main/security/national-labor-relations-board-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Employment
- Federal Government
- Labor
---
