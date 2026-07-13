---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unicamp.br
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.unicamp.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:56:08 2026 GMT
  host: redu.unicamp.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unicamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Campinas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: University of Campinas
provider_slug: unicamp
slug: unicamp-domain-security
source_filename: unicamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unicamp.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: redu.unicamp.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:56:08 2026 GMT\n  hsts: null\ndomains:\n- domain: unicamp.br\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicamp/refs/heads/main/security/unicamp-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Brazil
---
