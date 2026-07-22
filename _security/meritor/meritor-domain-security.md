---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meritor.com
  spf: true
hosts:
- cert_expires: Sep 25 03:58:45 2026 GMT
  host: www.meritor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meritor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meritor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: meritor
provider_slug: meritor
slug: meritor-domain-security
source_filename: meritor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meritor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:58:45 2026 GMT\n  hsts: false\ndomains:\n- domain: meritor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meritor/refs/heads/main/security/meritor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
---
