---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: truecare24.com
  spf: true
hosts:
- cert_expires: Oct  2 15:55:46 2026 GMT
  host: truecare24.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truecare24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueCare24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TrueCare24
provider_slug: truecare24
slug: truecare24-domain-security
source_filename: truecare24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truecare24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:55:46 2026 GMT\n  hsts: false\ndomains:\n- domain: truecare24.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truecare24/refs/heads/main/security/truecare24-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Home Care
- Healthcare Staffing
- Vaccinations
- Behavioral Health
---
