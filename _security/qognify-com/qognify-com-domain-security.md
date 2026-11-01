---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qognify.com
  spf: true
hosts:
- cert_expires: Dec 26 18:51:48 2026 GMT
  host: www.qognify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qognify Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qognify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qognify
provider_slug: qognify-com
slug: qognify-com-domain-security
source_filename: qognify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qognify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 18:51:48 2026 GMT\n  hsts: false\ndomains:\n- domain: qognify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/qognify-com/security/qognify-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- PublicSafety
- PhysicalSecurity
- VideoAnalytics
- AI
- Enterprise
---
