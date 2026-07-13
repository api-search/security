---
api_specs:
- filename: linguatools-collocations-openapi.yml
  format: yaml
  label: Linguatools Collocations API
  slug: collocations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linguatools/refs/heads/main/openapi/linguatools-collocations-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linguatools.org
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Aug 28 23:59:59 2026 GMT
  host: linguatools.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: linguatools-collocations.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Linguatools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linguatools, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Linguatools
provider_slug: linguatools
slug: linguatools-domain-security
source_filename: linguatools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linguatools.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:59:59 2026 GMT\n  hsts: false\n- host: linguatools-collocations.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: linguatools.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linguatools/refs/heads/main/security/linguatools-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Collocations
- Dictionary
- English
- Language
- Linguistics
- NLP
---
