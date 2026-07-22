---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buglance.com
  spf: true
hosts:
- cert_expires: Sep  6 20:30:46 2026 GMT
  host: buglance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glance Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buglance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buglance
provider_slug: glance-care
slug: glance-care-domain-security
source_filename: glance-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buglance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 20:30:46 2026 GMT\n  hsts: false\ndomains:\n- domain: buglance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glance-care/refs/heads/main/security/glance-care-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software Testing
- Quality Assurance
- Crowdsourced Testing
- Bug Reporting
- Mobile Testing
- Test Management
---
