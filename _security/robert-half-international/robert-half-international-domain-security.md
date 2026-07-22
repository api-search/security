---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roberthalf.com
  spf: true
hosts:
- cert_expires: Aug 28 08:52:11 2026 GMT
  host: www.roberthalf.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robert Half International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robert Half International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Robert Half International
provider_slug: robert-half-international
slug: robert-half-international-domain-security
source_filename: robert-half-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roberthalf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:52:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: roberthalf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robert-half-international/refs/heads/main/security/robert-half-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Staffing
- Recruiting
- Human Resources
- Talent Acquisition
- Finance
- Technology
- Fortune 1000
---
