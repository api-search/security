---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sptlabtech.com
  spf: true
hosts:
- cert_expires: Sep 18 08:29:26 2026 GMT
  host: www.sptlabtech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spt Labtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPT Labtech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SPT Labtech
provider_slug: spt-labtech
slug: spt-labtech-domain-security
source_filename: spt-labtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sptlabtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:29:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sptlabtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spt-labtech/refs/heads/main/security/spt-labtech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Laboratory Automation
- Liquid Handling
- Sample Management
- Drug Discovery
- Biotechnology
- Scientific Instruments
---
