---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rallypwr.com
  spf: true
hosts:
- cert_expires: Mar  2 01:43:03 2027 GMT
  host: rallypwr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rallypwr Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rally, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rally
provider_slug: rallypwr-com
slug: rallypwr-com-domain-security
source_filename: rallypwr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rallypwr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 01:43:03 2027 GMT\n  hsts: null\ndomains:\n- domain: rallypwr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rallypwr-com/security/rallypwr-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
