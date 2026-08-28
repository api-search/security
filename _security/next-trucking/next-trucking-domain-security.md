---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexttrucking.com
  spf: true
hosts:
- cert_expires: Sep 30 20:43:56 2026 GMT
  host: nexttrucking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: svcs.us-west-2.prod.aws.nexttrucking.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Next Trucking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NEXT Trucking, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NEXT Trucking
provider_slug: next-trucking
slug: next-trucking-domain-security
source_filename: next-trucking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexttrucking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:43:56 2026 GMT\n  hsts: false\n- host: svcs.us-west-2.prod.aws.nexttrucking.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nexttrucking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-trucking/refs/heads/main/security/next-trucking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Freight
- Trucking
- Drayage
- Supply Chain
- Transportation
- Marketplace
- Transportation Management
- Shipping
---
