---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: welocalize.com
  spf: true
hosts:
- cert_expires: Dec  3 14:20:57 2026 GMT
  host: welocalize.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Welocalize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opal by Welocalize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opal by Welocalize
provider_slug: welocalize
slug: welocalize-domain-security
source_filename: welocalize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: welocalize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 14:20:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: welocalize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/welocalize/security/welocalize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Localization
- AI
- Translation
- Enterprise
---
