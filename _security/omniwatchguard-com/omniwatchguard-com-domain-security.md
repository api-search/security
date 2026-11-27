---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omniwatchguard.com
  spf: true
hosts:
- cert_expires: Feb 12 14:35:38 2027 GMT
  host: omniwatchguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OmniWatchGuard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OmniWatchGuard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OmniWatchGuard
provider_slug: omniwatchguard-com
slug: omniwatchguard-com-domain-security
source_filename: omniwatchguard-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omniwatchguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 14:35:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: omniwatchguard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/omniwatchguard-com/security/omniwatchguard-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Automation
- Alerts
- Romania
- Software-as-a-Service
---
