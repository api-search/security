---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heymirza.com
  spf: true
hosts:
- cert_expires: Sep 28 02:00:01 2026 GMT
  host: heymirza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mirza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mirza
provider_slug: mirza
slug: mirza-domain-security
source_filename: mirza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heymirza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heymirza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirza/refs/heads/main/security/mirza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Public Benefits
- Government
- Healthcare
- Medicaid
- Eligibility
- Compliance
- Public Sector
---
