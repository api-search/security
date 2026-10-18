---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allonnia.com
  spf: true
hosts:
- cert_expires: Nov 25 22:27:57 2026 GMT
  host: allonnia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allonnia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allonnia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Allonnia
provider_slug: allonnia
slug: allonnia-domain-security
source_filename: allonnia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allonnia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:27:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: allonnia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allonnia/refs/heads/main/security/allonnia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Materials
- Sustainability
- Artificial Intelligence
- Mining
---
