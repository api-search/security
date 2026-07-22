---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cur8.earth
  spf: true
hosts:
- cert_expires: Oct 15 08:46:00 2026 GMT
  host: cur8.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cur8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cur8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cur8
provider_slug: cur8
slug: cur8-domain-security
source_filename: cur8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cur8.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cur8.earth\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cur8/refs/heads/main/security/cur8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Carbon Removal
- Climate
- Sustainability
- Carbon Credits
- Net Zero
- Climate Tech
---
