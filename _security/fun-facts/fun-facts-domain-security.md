---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: herokuapp.com
  spf: false
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: asli-fun-fact-api.herokuapp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fun Facts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fun Facts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Fun Facts
provider_slug: fun-facts
slug: fun-facts-domain-security
source_filename: fun-facts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asli-fun-fact-api.herokuapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: herokuapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fun-facts/refs/heads/main/security/fun-facts-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Games And Comics
- Public APIs
---
