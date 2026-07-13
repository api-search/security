---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: disify.com
  spf: true
hosts:
- cert_expires: Sep 25 16:39:56 2026 GMT
  host: www.disify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Disify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Disify
provider_slug: disify
slug: disify-domain-security
source_filename: disify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.disify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:39:56 2026 GMT\n  hsts: false\ndomains:\n- domain: disify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disify/refs/heads/main/security/disify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Public APIs
---
