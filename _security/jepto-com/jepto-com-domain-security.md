---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jepto.com
  spf: true
hosts:
- cert_expires: Feb  9 12:07:02 2027 GMT
  host: jepto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jepto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jepto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jepto
provider_slug: jepto-com
slug: jepto-com-domain-security
source_filename: jepto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jepto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 12:07:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jepto.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jepto-com/security/jepto-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketing
- Analytics
- Artificial Intelligence
- Reporting
- Integration
---
