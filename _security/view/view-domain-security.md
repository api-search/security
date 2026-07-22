---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: view.com
  spf: true
hosts:
- cert_expires: Sep 14 10:11:05 2026 GMT
  host: view.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: View Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for View, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: View
provider_slug: view
slug: view-domain-security
source_filename: view-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: view.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:11:05 2026 GMT\n  hsts: false\ndomains:\n- domain: view.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/view/refs/heads/main/security/view-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Proptech
- Smart Glass
- Smart Buildings
- IoT
- Electrochromic
- Building Automation
- Real Estate
---
