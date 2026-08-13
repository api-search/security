---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: easyknock.com
  spf: true
hosts:
- cert_expires: Sep 23 11:34:54 2026 GMT
  host: www.easyknock.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easyknock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyKnock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EasyKnock
provider_slug: easyknock
slug: easyknock-domain-security
source_filename: easyknock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.easyknock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:34:54 2026 GMT\n  hsts: false\ndomains:\n- domain: easyknock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyknock/refs/heads/main/security/easyknock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defunct
- Real Estate
- PropTech
- Fintech
- Sale Leaseback
- Home Equity
- Mortgage
- Consumer Finance
---
