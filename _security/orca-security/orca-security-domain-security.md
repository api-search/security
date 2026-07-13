---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orca.security
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orcasecurity.io
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: orca.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:32:11 2026 GMT
  host: docs.orcasecurity.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orca Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orca Security, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orca Security
provider_slug: orca-security
slug: orca-security-domain-security
source_filename: orca-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orca.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.orcasecurity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:32:11 2026 GMT\n  hsts: false\ndomains:\n- domain: orca.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: orcasecurity.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orca-security/refs/heads/main/security/orca-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentless
- API Security
- CIEM
- Cloud Security
- CNAPP
- CSPM
- CWPP
- DSPM
- SideScanning
- Vulnerability Management
---
