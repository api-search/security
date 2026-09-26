---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anlaiye.com
  spf: false
hosts:
- cert_expires: Oct 17 06:38:17 2026 GMT
  host: www.anlaiye.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anlaiye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anlaiye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Anlaiye
provider_slug: anlaiye
slug: anlaiye-domain-security
source_filename: anlaiye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anlaiye.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 06:38:17 2026 GMT\n  hsts: false\ndomains:\n- domain: anlaiye.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anlaiye/refs/heads/main/security/anlaiye-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
