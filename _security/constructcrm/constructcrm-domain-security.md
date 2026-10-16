---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: constructcrm.com
  spf: true
hosts:
- cert_expires: Dec 22 17:29:46 2026 GMT
  host: constructcrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constructcrm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConstructCRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ConstructCRM
provider_slug: constructcrm
slug: constructcrm-domain-security
source_filename: constructcrm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constructcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 17:29:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: constructcrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructcrm/refs/heads/main/security/constructcrm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
