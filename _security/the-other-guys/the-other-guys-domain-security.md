---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: other-guys.com
  spf: true
hosts:
- cert_expires: Jan 28 10:35:22 2027 GMT
  host: other-guys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Other Guys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Other Guys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Other Guys
provider_slug: the-other-guys
slug: the-other-guys-domain-security
source_filename: the-other-guys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: other-guys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:35:22 2027 GMT\n  hsts: null\ndomains:\n- domain: other-guys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-other-guys/refs/heads/main/security/the-other-guys-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
