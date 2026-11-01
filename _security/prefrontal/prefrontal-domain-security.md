---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prefrontal.ai
  spf: true
hosts:
- cert_expires: Dec 20 20:01:53 2026 GMT
  host: prefrontal.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prefrontal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prefrontal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prefrontal
provider_slug: prefrontal
slug: prefrontal-domain-security
source_filename: prefrontal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prefrontal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 20:01:53 2026 GMT\n  hsts: false\ndomains:\n- domain: prefrontal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/prefrontal/security/prefrontal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Data-Analytics
- Platform
- Enterprise
---
