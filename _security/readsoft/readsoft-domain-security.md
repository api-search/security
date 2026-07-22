---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tungstenautomation.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.tungstenautomation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Readsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReadSoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReadSoft
provider_slug: readsoft
slug: readsoft-domain-security
source_filename: readsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tungstenautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tungstenautomation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readsoft/refs/heads/main/security/readsoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts Payable
- Business Process Automation
- Document Processing
- Enterprise Software
- Invoice Processing
- OCR
- Capture
---
