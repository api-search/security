---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ceps.eu
  spf: true
hosts:
- cert_expires: Aug 17 16:06:52 2026 GMT
  host: www.ceps.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CEPS (Centre for European Policy Studies), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CEPS (Centre for European Policy Studies)
provider_slug: ceps
slug: ceps-domain-security
source_filename: ceps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ceps.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:06:52 2026 GMT\n  hsts: false\ndomains:\n- domain: ceps.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceps/refs/heads/main/security/ceps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Brussels
- Data Governance
- EU Policy
- European Union
- Policy Research
- Publications
- RSS
- Research
- Think Tank
---
