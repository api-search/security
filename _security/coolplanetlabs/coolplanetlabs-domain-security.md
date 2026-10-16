---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coolplanetlabs.org
  spf: true
hosts:
- cert_expires: Nov 30 21:50:13 2026 GMT
  host: coolplanetlabs.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coolplanetlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coolplanetlabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coolplanetlabs
provider_slug: coolplanetlabs
slug: coolplanetlabs-domain-security
source_filename: coolplanetlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coolplanetlabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 21:50:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coolplanetlabs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coolplanetlabs/refs/heads/main/security/coolplanetlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Education
- Nonprofit
- Community
- Sustainability
---
