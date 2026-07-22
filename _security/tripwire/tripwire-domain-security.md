---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tripwire.com
  spf: true
hosts:
- cert_expires: Aug 31 04:14:08 2026 GMT
  host: www.tripwire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripwire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripwire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tripwire
provider_slug: tripwire
slug: tripwire-domain-security
source_filename: tripwire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tripwire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:14:08 2026 GMT\n  hsts: null\ndomains:\n- domain: tripwire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripwire/refs/heads/main/security/tripwire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- File Integrity Monitoring
- Security Configuration Management
- Vulnerability Management
- Compliance
- Security
---
