---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microchip.com
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: www.microchip.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Microchip Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microchip Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microchip Technology
provider_slug: microchip-com
slug: microchip-com-domain-security
source_filename: microchip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microchip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: microchip.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microchip-com/security/microchip-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
