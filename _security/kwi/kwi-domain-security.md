---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kwi.com
  spf: true
hosts:
- cert_expires: Sep 11 13:05:44 2026 GMT
  host: www.kwi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kwi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KWI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KWI
provider_slug: kwi
slug: kwi-domain-security
source_filename: kwi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kwi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:05:44 2026 GMT\n  hsts: false\ndomains:\n- domain: kwi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kwi/refs/heads/main/security/kwi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Point of Sale
- Unified Commerce
- Omnichannel
- Order Management
- Merchandising
- Loyalty
- CRM
- Retail Analytics
- SaaS
---
