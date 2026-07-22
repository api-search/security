---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: poms.com
  spf: true
hosts:
- cert_expires: Aug 16 20:25:48 2026 GMT
  host: www.poms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for POMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: POMS
provider_slug: poms
slug: poms-domain-security
source_filename: poms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.poms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:25:48 2026 GMT\n  hsts: false\ndomains:\n- domain: poms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poms/refs/heads/main/security/poms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Manufacturing Execution System
- MES
- Pharmaceutical
- Electronic Batch Records
- Life Sciences
- Biotech
---
