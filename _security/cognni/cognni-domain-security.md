---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cognni.com
  spf: true
hosts:
- cert_expires: Dec  8 22:36:16 2026 GMT
  host: www.cognni.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cognni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cognni
provider_slug: cognni
slug: cognni-domain-security
source_filename: cognni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 22:36:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cognni.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognni/refs/heads/main/security/cognni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Knowledge Management
- Generative AI
- Enterprise Software
- Collaboration
- Insights
---
