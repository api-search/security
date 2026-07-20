---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: altruist.com
  spf: true
hosts:
- cert_expires: Sep 22 19:26:32 2026 GMT
  host: altruist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altruist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altruist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Altruist
provider_slug: altruist
slug: altruist-domain-security
source_filename: altruist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altruist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:26:32 2026 GMT\n  hsts: false\ndomains:\n- domain: altruist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruist/refs/heads/main/security/altruist-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Custody
- Wealth Management
- Financial Advisors
- RIA
- Investing
- OAuth
---
