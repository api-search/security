---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: higuests.com
  spf: true
hosts:
- cert_expires: Aug 30 18:44:15 2026 GMT
  host: higuests.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Higuest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiGuest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HiGuest
provider_slug: higuest
slug: higuest-domain-security
source_filename: higuest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: higuests.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:44:15 2026 GMT\n  hsts: false\ndomains:\n- domain: higuests.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/higuest/refs/heads/main/security/higuest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hospitality
- Property Management
- Short-Term Rental
- Vacation Rental
- Travel
- Real Estate
- Dubai
---
