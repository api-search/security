---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crowdforce.io
  spf: false
hosts:
- cert_expires: Sep 26 18:17:28 2026 GMT
  host: crowdforce.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crowdforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdForce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CrowdForce
provider_slug: crowdforce
slug: crowdforce-domain-security
source_filename: crowdforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdforce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:17:28 2026 GMT\n  hsts: false\ndomains:\n- domain: crowdforce.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdforce/refs/heads/main/security/crowdforce-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Payments
- Agent Banking
- Financial Inclusion
- Nigeria
- Africa
---
