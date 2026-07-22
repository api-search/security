---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dembiopharma.com
  spf: true
hosts:
- cert_expires: Sep  5 10:10:57 2026 GMT
  host: dembiopharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dem Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DEM Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DEM Bio
provider_slug: dem-bio
slug: dem-bio-domain-security
source_filename: dem-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dembiopharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 10:10:57 2026 GMT\n  hsts: false\ndomains:\n- domain: dembiopharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dem-bio/refs/heads/main/security/dem-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech Therapeutics
- Oncology
- Immunotherapy
- Cancer
- CRISPR
- Drug Discovery
- Functional Genomics
- Macrophage
---
