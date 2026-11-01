---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: flashpoint-intel.com
  spf: true
hosts:
- cert_expires: Dec 13 03:29:53 2026 GMT
  host: www.flashpoint-intel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flashpoint Intel Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flashpoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Flashpoint
provider_slug: flashpoint-intel-com
slug: flashpoint-intel-com-domain-security
source_filename: flashpoint-intel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flashpoint-intel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 03:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flashpoint-intel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flashpoint-intel-com/security/flashpoint-intel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Threat Intelligence
- Data Analytics
- API
---
