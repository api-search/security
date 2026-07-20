---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: labstep.com
  spf: true
hosts:
- cert_expires: Sep 10 18:56:25 2026 GMT
  host: www.labstep.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 16:06:06 2026 GMT
  host: help.labstep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.labstep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labstep, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Labstep
provider_slug: labstep
slug: labstep-domain-security
source_filename: labstep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.labstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:56:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.labstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:06:06 2026 GMT\n  hsts: false\n- host: api.labstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: labstep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labstep/refs/heads/main/security/labstep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electronic Lab Notebook
- Life Sciences
- Laboratory
- Research Data Management
- Scientific Software
- Inventory Management
- Biotechnology
- Chemistry
- Compliance
---
