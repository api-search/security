---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getagentwiki.com
  spf: true
hosts:
- cert_expires: Dec 22 04:46:07 2026 GMT
  host: getagentwiki.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Wiki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Wiki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agent Wiki
provider_slug: getagentwiki-com
slug: getagentwiki-com-domain-security
source_filename: getagentwiki-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getagentwiki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 04:46:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getagentwiki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getagentwiki-com/security/getagentwiki-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Collaboration
- Knowledge Management
- Wiki
---
