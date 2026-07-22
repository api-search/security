---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rimsys.io
  spf: true
hosts:
- cert_expires: Aug 30 20:31:58 2026 GMT
  host: www.rimsys.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 22:06:57 2026 GMT
  host: docs.rimsys.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.rimsys.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rimsys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rimsys, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rimsys
provider_slug: rimsys
slug: rimsys-domain-security
source_filename: rimsys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rimsys.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 20:31:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rimsys.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:06:57 2026 GMT\n  hsts: null\n- host: api.rimsys.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rimsys.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rimsys/refs/heads/main/security/rimsys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Regulatory
- Medical Devices
- MedTech
- Regulatory Information Management
- UDI
- Compliance
- Life Sciences
---
