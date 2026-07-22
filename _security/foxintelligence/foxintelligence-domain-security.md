---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foxintelligence.io
  spf: true
hosts:
- cert_expires: Sep 13 03:24:37 2026 GMT
  host: www.foxintelligence.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foxintelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foxintelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Foxintelligence
provider_slug: foxintelligence
slug: foxintelligence-domain-security
source_filename: foxintelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxintelligence.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:24:37 2026 GMT\n  hsts: false\ndomains:\n- domain: foxintelligence.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foxintelligence/refs/heads/main/security/foxintelligence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Applicative Saas
- E-Commerce
- Consumer Insights
- Retail Data
- Market Research
- Data Analytics
- Panel Data
---
