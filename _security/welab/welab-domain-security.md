---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: welab.co
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 iodef "mailto:cybersecurity@welab.bank"
  - 0 issue "comodoca.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: welab.bank
  spf: true
hosts:
- cert_expires: Oct  1 09:15:26 2026 GMT
  host: www.welab.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:15:32 2026 GMT
  host: portal-sandbox.welab.bank
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.welab.bank
  https: false
kind: domain-security
layout: security
method: probed
name: Welab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeLab, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WeLab
provider_slug: welab
slug: welab-domain-security
source_filename: welab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.welab.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:15:26 2026 GMT\n  hsts: false\n- host: portal-sandbox.welab.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:15:32 2026 GMT\n  hsts: null\n- host: api.welab.bank\n  https: false\ndomains:\n- domain: welab.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: welab.bank\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 iodef \"mailto:cybersecurity@welab.bank\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welab/refs/heads/main/security/welab-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fintech
- Digital Banking
- virtual-bank
- Open Banking
- Hong Kong
- Indonesia
- Consumer Lending
- Payments
- hkma-open-api
- Financial-Services
---
