---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itasoftware.com
  spf: true
hosts:
- cert_expires: Sep 21 08:39:43 2026 GMT
  host: www.itasoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ita Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ITA Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ITA Software
provider_slug: ita-software
slug: ita-software-domain-security
source_filename: ita-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itasoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:39:43 2026 GMT\n  hsts: false\ndomains:\n- domain: itasoftware.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ita-software/refs/heads/main/security/ita-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Airlines
- Airfare
- Flight Search
- Travel Technology
- Pricing
- Google
---
