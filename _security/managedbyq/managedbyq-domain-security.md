---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: managedbyq.com
  spf: false
hosts:
- cert_expires: Sep 13 07:44:51 2026 GMT
  host: managedbyq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Managedbyq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for managedbyq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: managedbyq
provider_slug: managedbyq
slug: managedbyq-domain-security
source_filename: managedbyq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: managedbyq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:44:51 2026 GMT\n  hsts: false\ndomains:\n- domain: managedbyq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/managedbyq/refs/heads/main/security/managedbyq-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
