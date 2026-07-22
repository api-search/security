---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daffy.org
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.daffy.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Daffy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daffy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daffy
provider_slug: daffy
slug: daffy-domain-security
source_filename: daffy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daffy.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: daffy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daffy/refs/heads/main/security/daffy-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Charitable Giving
- Donor Advised Fund
- Nonprofit
- Wealth Management
- Investing
- Philanthropy
---
