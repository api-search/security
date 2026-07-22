---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ndata.cz
  spf: true
hosts:
- cert_expires: Sep 12 15:01:22 2026 GMT
  host: www.ndata.cz
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ndata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ndata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ndata
provider_slug: ndata
slug: ndata-domain-security
source_filename: ndata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ndata.cz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 12 15:01:22 2026 GMT\n  hsts: false\ndomains:\n- domain: ndata.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ndata/refs/heads/main/security/ndata-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Pharmaceutical
- Regulatory Affairs
- Quality Management
- Compliance
- Clinical Trials
- Life Sciences
- GxP
- Software
---
