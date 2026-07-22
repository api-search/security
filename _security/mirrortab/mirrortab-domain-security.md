---
api_specs:
- filename: mirrortab-api-openapi.yml
  format: yaml
  label: MirrorTab API
  slug: mirrortab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirrortab/refs/heads/main/openapi/mirrortab-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mirrortab.com
  spf: true
hosts:
- cert_expires: Sep 14 08:17:33 2026 GMT
  host: www.mirrortab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.mirrortab.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mirrortab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MirrorTab, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MirrorTab
provider_slug: mirrortab
slug: mirrortab-domain-security
source_filename: mirrortab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mirrortab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:17:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mirrortab.com\n  https: false\ndomains:\n- domain: mirrortab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirrortab/refs/heads/main/security/mirrortab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Security
- Cybersecurity
- Bot Mitigation
- Fraud Prevention
- Browser Isolation
- Anti-Automation
---
