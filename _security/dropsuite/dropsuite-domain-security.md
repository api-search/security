---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dropsuite.com
  spf: true
hosts:
- cert_expires: Aug 26 11:14:24 2026 GMT
  host: dropsuite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dropsuite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropsuite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dropsuite
provider_slug: dropsuite
slug: dropsuite-domain-security
source_filename: dropsuite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dropsuite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:14:24 2026 GMT\n  hsts: false\ndomains:\n- domain: dropsuite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropsuite/refs/heads/main/security/dropsuite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Backup
- Data Protection
- Email Archiving
- Microsoft 365
- Google Workspace
- MSP
- Compliance
- eDiscovery
- Disaster Recovery
---
