---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: synonyms.com
  spf: false
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.synonyms.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Synonyms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synonyms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Synonyms
provider_slug: synonyms
slug: synonyms-domain-security
source_filename: synonyms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synonyms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: synonyms.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synonyms/refs/heads/main/security/synonyms-domain-security.yml
summary_line: TLSv1.2
tags:
- Dictionaries
- Public APIs
---
