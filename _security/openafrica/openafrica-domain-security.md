---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: africaopendata.org
  spf: false
hosts:
- cert_expires: Sep  1 14:06:15 2026 GMT
  host: africaopendata.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openafrica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openAFRICA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: openAFRICA
provider_slug: openafrica
slug: openafrica-domain-security
source_filename: openafrica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: africaopendata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:06:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: africaopendata.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openafrica/refs/heads/main/security/openafrica-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- Public APIs
---
