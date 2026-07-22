---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eqlfinance.com
  spf: true
hosts:
- cert_expires: Oct 12 23:44:45 2026 GMT
  host: eqlfinance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eql Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EQL Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EQL Finance
provider_slug: eql-finance
slug: eql-finance-domain-security
source_filename: eql-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eqlfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:44:45 2026 GMT\n  hsts: null\ndomains:\n- domain: eqlfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eql-finance/refs/heads/main/security/eql-finance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
