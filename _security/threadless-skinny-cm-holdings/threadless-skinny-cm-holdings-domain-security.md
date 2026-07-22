---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: threadless.com
  spf: true
hosts:
- cert_expires: Oct 10 17:47:15 2026 GMT
  host: www.threadless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Threadless Skinny Cm Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Threadless ( Skinny CM Holdings), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Threadless ( Skinny CM Holdings)
provider_slug: threadless-skinny-cm-holdings
slug: threadless-skinny-cm-holdings-domain-security
source_filename: threadless-skinny-cm-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.threadless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:47:15 2026 GMT\n  hsts: null\ndomains:\n- domain: threadless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threadless-skinny-cm-holdings/refs/heads/main/security/threadless-skinny-cm-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Apparel
- E-commerce
- Marketplace
- Print on Demand
- Design Community
---
