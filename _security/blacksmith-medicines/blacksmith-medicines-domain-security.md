---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blacksmithmedicines.com
  spf: true
hosts:
- cert_expires: Dec 19 07:25:16 2026 GMT
  host: blacksmithmedicines.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blacksmith Medicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blacksmith Medicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Blacksmith Medicines
provider_slug: blacksmith-medicines
slug: blacksmith-medicines-domain-security
source_filename: blacksmith-medicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blacksmithmedicines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 07:25:16 2026 GMT\n  hsts: false\ndomains:\n- domain: blacksmithmedicines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksmith-medicines/refs/heads/main/security/blacksmith-medicines-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharma
- Metalloenzyme
- Drug Discovery
- San Diego
---
