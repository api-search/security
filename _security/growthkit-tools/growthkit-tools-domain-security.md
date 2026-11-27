---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: growthkit.tools
  spf: false
hosts:
- cert_expires: Jan 17 11:17:52 2027 GMT
  host: growthkit.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GrowthKit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrowthKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: GrowthKit
provider_slug: growthkit-tools
slug: growthkit-tools-domain-security
source_filename: growthkit-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: growthkit.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 11:17:52 2027 GMT\n  hsts: false\ndomains:\n- domain: growthkit.tools\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/growthkit-tools/security/growthkit-tools-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Software-as-a-Service
- Marketing
- Sales
- Consulting
- Growth
---
