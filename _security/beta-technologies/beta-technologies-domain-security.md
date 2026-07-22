---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beta.team
  spf: true
hosts:
- cert_expires: Sep 19 00:15:49 2026 GMT
  host: www.beta.team
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beta Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BETA Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BETA Technologies
provider_slug: beta-technologies
slug: beta-technologies-domain-security
source_filename: beta-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beta.team\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:15:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beta.team\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beta-technologies/refs/heads/main/security/beta-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advanced Air Mobility
- Aerospace
- Charging Infrastructure
- Defense
- eVTOL
- eCTOL
- Electric Aviation
- FAA Certification
- Manufacturing
- Sustainable Aviation
---
