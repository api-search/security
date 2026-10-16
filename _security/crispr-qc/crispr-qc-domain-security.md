---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crisprqc.com
  spf: true
hosts:
- cert_expires: Nov 17 02:08:36 2026 GMT
  host: crisprqc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crispr Qc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRISPR QC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CRISPR QC
provider_slug: crispr-qc
slug: crispr-qc-domain-security
source_filename: crispr-qc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crisprqc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 02:08:36 2026 GMT\n  hsts: false\ndomains:\n- domain: crisprqc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crispr-qc/refs/heads/main/security/crispr-qc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Gene Editing
- Analytics
- Platform
---
