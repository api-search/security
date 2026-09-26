---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atomberg.com
  spf: true
hosts:
- cert_expires: Nov 15 15:24:32 2026 GMT
  host: atomberg.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atombergtechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atombergtechnology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atombergtechnology
provider_slug: atombergtechnology
slug: atombergtechnology-domain-security
source_filename: atombergtechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 15:24:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: atomberg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atombergtechnology/refs/heads/main/security/atombergtechnology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SmartHome
- Appliances
- India
- EnergyEfficient
---
