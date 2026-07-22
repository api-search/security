---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coopertire.com
  spf: true
hosts:
- cert_expires: Sep 28 16:58:53 2026 GMT
  host: www.coopertire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cooper Tire And Rubber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cooper Tire & Rubber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cooper Tire & Rubber
provider_slug: cooper-tire-and-rubber
slug: cooper-tire-and-rubber-domain-security
source_filename: cooper-tire-and-rubber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coopertire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:58:53 2026 GMT\n  hsts: false\ndomains:\n- domain: coopertire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooper-tire-and-rubber/refs/heads/main/security/cooper-tire-and-rubber-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Acquired
- Aftermarket
- Automotive
- Consumer
- Goodyear
- Manufacturing
- Replacement Tires
- Tires
- Fortune 1000
---
