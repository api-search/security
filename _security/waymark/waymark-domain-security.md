---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: waymarkcare.com
  spf: true
hosts:
- cert_expires: Oct  1 08:31:49 2026 GMT
  host: www.waymarkcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waymark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waymark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Waymark
provider_slug: waymark
slug: waymark-domain-security
source_filename: waymark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.waymarkcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:31:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: waymarkcare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waymark/refs/heads/main/security/waymark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Medicaid
- Community Health
- Value-Based Care
- Care Coordination
- Population Health
---
