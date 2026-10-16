---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bridgeinternationalacademies.com
  spf: false
hosts:
- cert_expires: Dec 15 00:34:45 2026 GMT
  host: www.bridgeinternationalacademies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bridgeinternationalacademies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridgeinternationalacademies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Bridgeinternationalacademies
provider_slug: bridgeinternationalacademies
slug: bridgeinternationalacademies-domain-security
source_filename: bridgeinternationalacademies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bridgeinternationalacademies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 00:34:45 2026 GMT\n  hsts: false\ndomains:\n- domain: bridgeinternationalacademies.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgeinternationalacademies/refs/heads/main/security/bridgeinternationalacademies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
