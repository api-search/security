---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: doradosoftware.com
  spf: true
hosts:
- cert_expires: Sep 14 02:36:19 2026 GMT
  host: www.doradosoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dorado Software Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dorado Software Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dorado Software Inc
provider_slug: dorado-software-inc
slug: dorado-software-inc-domain-security
source_filename: dorado-software-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doradosoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:36:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doradosoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dorado-software-inc/refs/heads/main/security/dorado-software-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure Management
- Network Management
- DCIM
- Orchestration
- Monitoring
- Data Center
- AIOps
---
