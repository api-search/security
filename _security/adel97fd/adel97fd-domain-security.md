---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adelpharm.com
  spf: true
hosts:
- cert_expires: Nov 15 15:15:19 2026 GMT
  host: adelpharm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adel97Fd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADEL, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ADEL, Inc.
provider_slug: adel97fd
slug: adel97fd-domain-security
source_filename: adel97fd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adelpharm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 15:15:19 2026 GMT\n  hsts: false\ndomains:\n- domain: adelpharm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nnote: >-\n  probe-domain-security.py probed only adelpharm.com because that is the sole host in apis.yml.\n  The company's other first-party hosts (www.adelpharm.com, adelbio.com, www.adelbio.com,\n  adelbio.co.kr, www.adelbio.co.kr) all resolve to the same Cafe24 origin 183.111.183.82 and\n  share the same nameservers, so the same posture applies. Findings: TLS 1.2 only (no TLS 1.3\n  negotiated), no HSTS, no DNSSEC, no CAA record, SPF present, no DMARC record. Absence of a\n  record is observed data, not an inference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adel97fd/refs/heads/main/security/adel97fd-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Healthcare
- Drug Discovery
- Antibody Therapeutics
- Neuroscience
- Alzheimers Disease
- Clinical Trials
- Diagnostics
- South Korea
---
