---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:admin@hud.gov"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hud.gov
  spf: true
hosts:
- cert_expires: Sep  7 14:57:29 2026 GMT
  host: www.hud.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fair Housing And Equal Opportunity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fair Housing and Equal Opportunity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fair Housing and Equal Opportunity
provider_slug: fair-housing-and-equal-opportunity
slug: fair-housing-and-equal-opportunity-domain-security
source_filename: fair-housing-and-equal-opportunity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hud.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:57:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hud.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:admin@hud.gov\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fair-housing-and-equal-opportunity/refs/heads/main/security/fair-housing-and-equal-opportunity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Equal Opportunity
- Fair Housing
- Federal Government
- Housing
- HUD
---
