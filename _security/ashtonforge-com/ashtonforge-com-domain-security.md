---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ashtonforge.com
  spf: true
hosts:
- cert_expires: Jan 15 04:32:38 2027 GMT
  host: ashtonforge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ashton & Forge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ashton & Forge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ashton & Forge
provider_slug: ashtonforge-com
slug: ashtonforge-com-domain-security
source_filename: ashtonforge-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ashtonforge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 04:32:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ashtonforge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ashtonforge-com/security/ashtonforge-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Marketplace
- Agency
- Matching
- Platform
- Company
---
