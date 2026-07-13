---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.es
  spf: false
hosts:
- cert_expires: Mar  3 17:48:31 2027 GMT
  host: datos.gob.es
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Spain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Spain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Open Government, Spain
provider_slug: open-government-spain
slug: open-government-spain-domain-security
source_filename: open-government-spain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.gob.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 17:48:31 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: gob.es\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-spain/refs/heads/main/security/open-government-spain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Public APIs
---
