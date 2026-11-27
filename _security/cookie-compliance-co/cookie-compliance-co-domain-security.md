---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cookie-compliance.co
  spf: true
hosts:
- cert_expires: Dec  6 21:20:00 2026 GMT
  host: cookie-compliance.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cookie Compliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cookie Compliance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cookie Compliance
provider_slug: cookie-compliance-co
slug: cookie-compliance-co-domain-security
source_filename: cookie-compliance-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cookie-compliance.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 21:20:00 2026 GMT\n  hsts: false\ndomains:\n- domain: cookie-compliance.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cookie-compliance-co/security/cookie-compliance-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cookie Consent
- Consent Management
- Privacy
- GDPR
- CCPA
- Compliance
- MCP
---
