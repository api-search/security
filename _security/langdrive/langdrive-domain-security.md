---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: addyai.com
  spf: true
hosts:
- cert_expires: May  2 05:06:01 2027 GMT
  host: www.addyai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Langdrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Addy AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Addy AI
provider_slug: langdrive
slug: langdrive-domain-security
source_filename: langdrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.addyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  2 05:06:01 2027 GMT\n  hsts: null\ndomains:\n- domain: addyai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/langdrive/security/langdrive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Mortgage
- Automation
- FinTech
---
