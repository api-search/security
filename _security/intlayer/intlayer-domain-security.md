---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: intlayer.org
  spf: true
hosts:
- cert_expires: Nov 15 05:38:58 2026 GMT
  host: intlayer.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intlayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Intlayer
provider_slug: intlayer
slug: intlayer-domain-security
source_filename: intlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intlayer.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 05:38:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intlayer.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intlayer/refs/heads/main/security/intlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- i18n
- Internationalization
- Localization
- React
- Next.js
- CMS
- MCP
---
