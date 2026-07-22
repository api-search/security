---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unicomengineering.com
  spf: true
  spf_record: v=spf1 mx include:spf.protection.outlook.com include:securityiqmail.net include:mktomail.com include:spf.emailsignatures365.com include:_spf-amer.onbmc.com ~all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: networkengines.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- host: www.unicomengineering.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: networkengines.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  redirects_to: https://www.unicomengineering.com/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Network Engines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Network Engines, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Network Engines
provider_slug: network-engines
slug: network-engines-domain-security
source_filename: network-engines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + openssl s_client + curl HEAD (live probe)\nnote: >-\n  Network Engines Inc. was acquired by UNICOM Global and rebranded UNICOM\n  Engineering; networkengines.com now redirects to www.unicomengineering.com.\n  These are the corporate marketing hosts — the company publishes no public API,\n  so this domain-security probe covers only the corporate web/mail domains.\nhosts:\n- host: www.unicomengineering.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n- host: networkengines.com\n  https: true\n  redirects_to: https://www.unicomengineering.com/\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unicomengineering.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 mx include:spf.protection.outlook.com include:securityiqmail.net include:mktomail.com include:spf.emailsignatures365.com include:_spf-amer.onbmc.com ~all\"\n  dmarc: true\n  dmarc_policy:\
  \ none\n- domain: networkengines.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 include:spf.protection.outlook.com -all\"\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/network-engines/refs/heads/main/security/network-engines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Server Appliances
- OEM
- Systems Integration
- Application Platforms
- Enterprise Infrastructure
---
