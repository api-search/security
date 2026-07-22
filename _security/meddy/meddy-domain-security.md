---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meddy.co
  spf: true
hosts:
- cert_expires: Sep  3 09:05:13 2026 GMT
  host: meddy.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meddy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meddy
provider_slug: meddy
slug: meddy-domain-security
source_filename: meddy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meddy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:05:13 2026 GMT\n  hsts: false\ndomains:\n- domain: meddy.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meddy/refs/heads/main/security/meddy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
