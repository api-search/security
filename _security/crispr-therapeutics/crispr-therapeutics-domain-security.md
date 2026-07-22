---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crisprtx.com
  spf: true
hosts:
- cert_expires: Oct  7 06:16:40 2026 GMT
  host: www.crisprtx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crispr Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRISPR Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CRISPR Therapeutics
provider_slug: crispr-therapeutics
slug: crispr-therapeutics-domain-security
source_filename: crispr-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crisprtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 06:16:40 2026 GMT\n  hsts: false\ndomains:\n- domain: crisprtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crispr-therapeutics/refs/heads/main/security/crispr-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Gene Editing
- CRISPR
- Genomics
- Pharmaceuticals
---
