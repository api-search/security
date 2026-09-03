---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: yellowbrink.com
  spf: true
hosts:
- cert_expires: Oct 16 12:01:38 2026 GMT
  host: www.yellowbrink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yellowbrink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YellowBrink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: YellowBrink
provider_slug: yellowbrink
slug: yellowbrink-domain-security
source_filename: yellowbrink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yellowbrink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yellowbrink.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yellowbrink/refs/heads/main/security/yellowbrink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health Care
- Health Data
- openEHR
- Interoperability
- Standards
- Community
- Education
- Events
- Netherlands
---
