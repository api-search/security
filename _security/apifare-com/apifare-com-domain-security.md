---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apifare.com
  spf: true
hosts:
- cert_expires: Dec 10 10:30:46 2026 GMT
  host: apifare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apifare Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apifare-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: apifare-com
provider_slug: apifare-com
slug: apifare-com-domain-security
source_filename: apifare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apifare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 10:30:46 2026 GMT\n  hsts: false\ndomains:\n- domain: apifare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/apifare-com/security/apifare-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Payments
- Prepaid
- Billing
- Agent
---
