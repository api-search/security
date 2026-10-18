---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: konantech.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: konantech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Konantech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konan Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Konan Technology
provider_slug: konantech
slug: konantech-domain-security
source_filename: konantech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konantech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: konantech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konantech/refs/heads/main/security/konantech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
