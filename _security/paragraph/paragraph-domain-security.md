---
api_specs:
- filename: paragraph-openapi-original.json
  format: json
  label: Paragraph API
  slug: paragraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paragraph.xyz
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paragraph.com
  spf: true
hosts:
- cert_expires: Sep  1 21:35:00 2026 GMT
  host: paragraph.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 02:46:09 2026 GMT
  host: public.api.paragraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paragraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paragraph, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paragraph
provider_slug: paragraph
slug: paragraph-domain-security
source_filename: paragraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paragraph.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:35:00 2026 GMT\n  hsts: false\n- host: public.api.paragraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 02:46:09 2026 GMT\n  hsts: null\ndomains:\n- domain: paragraph.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: paragraph.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/security/paragraph-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Publishing
- Newsletters
- Web3
- Content
- Blogging
- Creator Economy
- API
---
