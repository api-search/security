---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: leg.br
  spf: false
hosts:
- cert_expires: Sep 26 12:10:02 2026 GMT
  host: dadosabertos.camara.leg.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brazilian Chamber Of Deputies Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brazilian Chamber of Deputies Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Brazilian Chamber of Deputies Open Data
provider_slug: brazilian-chamber-of-deputies-open-data
slug: brazilian-chamber-of-deputies-open-data-domain-security
source_filename: brazilian-chamber-of-deputies-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dadosabertos.camara.leg.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:10:02 2026 GMT\n  hsts: false\ndomains:\n- domain: leg.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brazilian-chamber-of-deputies-open-data/refs/heads/main/security/brazilian-chamber-of-deputies-open-data-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Government
- Public APIs
---
