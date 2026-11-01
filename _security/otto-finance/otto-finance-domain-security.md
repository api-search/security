---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:info@ottofinance.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ottofinance.io
  spf: true
hosts:
- cert_expires: Jan  8 18:02:33 2027 GMT
  host: www.ottofinance.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Otto Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otto Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Otto Finance
provider_slug: otto-finance
slug: otto-finance-domain-security
source_filename: otto-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ottofinance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 18:02:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ottofinance.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:info@ottofinance.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/otto-finance/security/otto-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- FinTech
- Wealth Management
- Automation
- AI
---
