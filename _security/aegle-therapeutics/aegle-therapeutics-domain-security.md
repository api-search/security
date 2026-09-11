---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aegletherapeutics.com
  spf: true
hosts:
- cert_expires: Oct 19 19:33:53 2026 GMT
  host: aegletherapeutics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aegle Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aegle Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aegle Therapeutics
provider_slug: aegle-therapeutics
slug: aegle-therapeutics-domain-security
source_filename: aegle-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aegletherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 19:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aegletherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aegle-therapeutics/refs/heads/main/security/aegle-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Life Sciences
- Regenerative Medicine
- Clinical Stage
- Pharmaceuticals
- Rare Disease
- Health
---
