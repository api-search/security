---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alpha.com
  spf: true
hosts:
- cert_expires: Sep 11 23:56:33 2026 GMT
  host: www.alpha.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpha Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpha Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alpha Technologies
provider_slug: alpha-technologies
slug: alpha-technologies-domain-security
source_filename: alpha-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:56:33 2026 GMT\n  hsts: false\ndomains:\n- domain: alpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpha-technologies/refs/heads/main/security/alpha-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Power Systems
- Energy
- Telecommunications
- Hardware
- Renewable Energy
- Backup Power
---
