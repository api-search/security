---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aktana.com
  spf: true
hosts:
- cert_expires: Dec 30 18:30:31 2026 GMT
  host: aktana.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aktana Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aktana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aktana
provider_slug: aktana-com
slug: aktana-com-domain-security
source_filename: aktana-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aktana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 18:30:31 2026 GMT\n  hsts: false\ndomains:\n- domain: aktana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aktana-com/security/aktana-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Pharma Marketing
- HCP Engagement
- AI Insights
- Omnichannel
- Medical Affairs
---
