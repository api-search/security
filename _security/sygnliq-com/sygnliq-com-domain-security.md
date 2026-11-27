---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sygnliq.com
  spf: true
hosts:
- cert_expires: Feb 20 13:37:17 2027 GMT
  host: sygnliq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: sygnliq-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sygnliq-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: sygnliq-com
provider_slug: sygnliq-com
slug: sygnliq-com-domain-security
source_filename: sygnliq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sygnliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 13:37:17 2027 GMT\n  hsts: null\ndomains:\n- domain: sygnliq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sygnliq-com/security/sygnliq-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
