---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adspirer.com
  spf: true
hosts:
- cert_expires: Dec  7 03:30:24 2026 GMT
  host: adspirer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adspirer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adspirer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adspirer
provider_slug: adspirer-com
slug: adspirer-com-domain-security
source_filename: adspirer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adspirer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 03:30:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adspirer.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adspirer-com/security/adspirer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Advertising
- Paid Media
- MCP
- Marketing Automation
---
