---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aurionbiotech.com
  spf: true
hosts:
- cert_expires: Nov 11 06:18:42 2026 GMT
  host: aurionbiotech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurion Biotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurion Biotech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aurion Biotech
provider_slug: aurion-biotech
slug: aurion-biotech-domain-security
source_filename: aurion-biotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurionbiotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 06:18:42 2026 GMT\n  hsts: false\ndomains:\n- domain: aurionbiotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurion-biotech/refs/heads/main/security/aurion-biotech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biotechnology
- Ophthalmology
- Regenerative Medicine
- Cell Therapy
- Vision Restoration
- Company
---
