---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  - 0 iodef "mailto:sysadmins@lovecrafts.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lovecrafts.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.lovecrafts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lovecrafts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lovecrafts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: lovecrafts
provider_slug: lovecrafts
slug: lovecrafts-domain-security
source_filename: lovecrafts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lovecrafts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lovecrafts.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 iodef \"mailto:sysadmins@lovecrafts.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovecrafts/refs/heads/main/security/lovecrafts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crafts
- E-Commerce
- Retail
- Marketplace
- Community
- Patterns
- Consumer
---
