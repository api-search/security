---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: matterworksbio.com
  spf: true
hosts:
- cert_expires: Oct 13 23:56:37 2026 GMT
  host: www.matterworksbio.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matterworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matterworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Matterworks
provider_slug: matterworks
slug: matterworks-domain-security
source_filename: matterworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.matterworksbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: matterworksbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matterworks/refs/heads/main/security/matterworks-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Metabolomics
- Omics
- Life Sciences
- Biotechnology
- Mass Spectrometry
- Foundation Models
---
