---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: webfinanceholding.com
  spf: true
hosts:
- cert_expires: Sep 24 11:00:31 2026 GMT
  host: webfinanceholding.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webfinanceholding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webfinanceholding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Webfinanceholding
provider_slug: webfinanceholding
slug: webfinanceholding-domain-security
source_filename: webfinanceholding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webfinanceholding.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:00:31 2026 GMT\n  hsts: false\ndomains:\n- domain: webfinanceholding.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webfinanceholding/refs/heads/main/security/webfinanceholding-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Financial Services
- Holding Company
- Debt Portfolio Management
- Receivables
- Insurance
- Banking
- Bulgaria
---
