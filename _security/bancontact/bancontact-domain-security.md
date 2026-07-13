---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bancontact.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bancontactpro.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.bancontact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 07:05:35 2026 GMT
  host: docs.bancontactpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bancontact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bancontact, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bancontact
provider_slug: bancontact
slug: bancontact-domain-security
source_filename: bancontact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bancontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\n- host: docs.bancontactpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 07:05:35 2026 GMT\n  hsts: false\ndomains:\n- domain: bancontact.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bancontactpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/security/bancontact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- Belgium
- Debit Cards
- E-Commerce
- Fintech
- Payments
---
