---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cellresearchcorp.com
  spf: true
hosts:
- cert_expires: Dec 18 16:20:46 2026 GMT
  host: www.cellresearchcorp.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellresearch Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CellResearch Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CellResearch Corporation
provider_slug: cellresearch-corporation
slug: cellresearch-corporation-domain-security
source_filename: cellresearch-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cellresearchcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:20:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: cellresearchcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellresearch-corporation/refs/heads/main/security/cellresearch-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Stem-Cell
- Regenerative-Medicine
- Singapore
---
