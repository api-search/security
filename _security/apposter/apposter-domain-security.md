---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apposter.com
  spf: true
hosts:
- cert_expires: Nov 22 11:41:20 2026 GMT
  host: apposter.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apposter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apposter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apposter
provider_slug: apposter
slug: apposter-domain-security
source_filename: apposter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apposter.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 11:41:20 2026 GMT\n  hsts: false\ndomains:\n- domain: apposter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apposter/refs/heads/main/security/apposter-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Wearable Technology
- Smart Ring
---
