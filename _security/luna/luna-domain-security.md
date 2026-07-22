---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getluna.com
  spf: true
hosts:
- cert_expires: Oct 12 23:33:52 2026 GMT
  host: getluna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Luna
provider_slug: luna
slug: luna-domain-security
source_filename: luna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getluna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:33:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getluna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luna/refs/heads/main/security/luna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Physical Therapy
- In-Home Care
- Rehabilitation
- Digital Health
---
