---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chatgpt.site
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Jan 29 18:12:55 2027 GMT
  host: flamingo-api-guides.flatemu1.chatgpt.site
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: access-file-extractor.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: creativepack.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Flamingo APIs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flamingo APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flamingo APIs
provider_slug: flamingo-apis
slug: flamingo-apis-domain-security
source_filename: flamingo-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flamingo-api-guides.flatemu1.chatgpt.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 18:12:55 2027 GMT\n  hsts: false\n- host: access-file-extractor.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n- host: creativepack.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: chatgpt.site\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flamingo-apis/security/flamingo-apis-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- File Processing
- Python
- RapidAPI
- WooCommerce
- Data Export
---
