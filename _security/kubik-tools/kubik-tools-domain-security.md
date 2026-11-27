---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kubik.tools
  spf: true
hosts:
- cert_expires: Dec 15 21:30:15 2026 GMT
  host: kubik.tools
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: kubik.tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kubik.tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: kubik.tools
provider_slug: kubik-tools
slug: kubik-tools-domain-security
source_filename: kubik-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubik.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 21:30:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubik.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kubik-tools/security/kubik-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Calculator
- Packing
- Browser
- Open Source
---
