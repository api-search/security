---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: auroraconcierge.com.br
  spf: false
hosts:
- cert_expires: Dec 25 19:52:15 2026 GMT
  host: auroraconcierge.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurora Concierge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurora Concierge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aurora Concierge
provider_slug: auroraconcierge-com-br
slug: auroraconcierge-com-br-domain-security
source_filename: auroraconcierge-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auroraconcierge.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 19:52:15 2026 GMT\n  hsts: null\ndomains:\n- domain: auroraconcierge.com.br\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/auroraconcierge-com-br/security/auroraconcierge-com-br-domain-security.yml
summary_line: TLSv1.3
tags:
- Home Care
- Healthcare
- Brazil
- Nursing
- Concierge
- Company
---
