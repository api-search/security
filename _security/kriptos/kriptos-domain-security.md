---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kriptos.io
  spf: true
hosts:
- cert_expires: Oct 14 07:28:53 2026 GMT
  host: kriptos.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kriptos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kriptos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kriptos
provider_slug: kriptos
slug: kriptos-domain-security
source_filename: kriptos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kriptos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kriptos.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kriptos/refs/heads/main/security/kriptos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Data Classification
- Data Loss Prevention
- Data Governance
- Compliance
- DSPM
- Insider Threat
- Artificial Intelligence
- Unstructured Data
- Microsoft 365
- Google Workspace
---
