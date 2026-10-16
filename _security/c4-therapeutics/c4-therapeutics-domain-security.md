---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: c4therapeutics.com
  spf: true
hosts:
- cert_expires: Dec 20 20:27:12 2026 GMT
  host: c4therapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: C4 Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C4 Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: C4 Therapeutics
provider_slug: c4-therapeutics
slug: c4-therapeutics-domain-security
source_filename: c4-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: c4therapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 20:27:12 2026 GMT\n  hsts: false\ndomains:\n- domain: c4therapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c4-therapeutics/refs/heads/main/security/c4-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharma
- Cancer
- Targeted Protein Degradation
- TORPEDO Platform
---
