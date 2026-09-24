---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ambri.com
  spf: true
hosts:
- cert_expires: Nov 21 22:08:31 2026 GMT
  host: ambri.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ambri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ambri
provider_slug: ambri
slug: ambri-domain-security
source_filename: ambri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 22:08:31 2026 GMT\n  hsts: false\ndomains:\n- domain: ambri.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambri/refs/heads/main/security/ambri-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Storage
- Battery
- Renewable
---
