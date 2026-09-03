---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: validusgrp.com
  spf: true
hosts:
- cert_expires: Oct 16 17:07:18 2026 GMT
  host: validusgrp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Validus Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Validus Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Validus Capital
provider_slug: validus-capital
slug: validus-capital-domain-security
source_filename: validus-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: validusgrp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:07:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: validusgrp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validus-capital/refs/heads/main/security/validus-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Lending
- SME Finance
- Fintech
- Supply Chain Finance
- Invoice Financing
- Working Capital
- Southeast Asia
- Singapore
---
