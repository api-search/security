---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upsidefoods.com
  spf: true
hosts:
- cert_expires: Sep 20 18:27:17 2026 GMT
  host: upsidefoods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upsidefoods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UPSIDE Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UPSIDE Foods
provider_slug: upsidefoods
slug: upsidefoods-domain-security
source_filename: upsidefoods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upsidefoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:27:17 2026 GMT\n  hsts: false\ndomains:\n- domain: upsidefoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsidefoods/refs/heads/main/security/upsidefoods-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Cultivated Meat
- Food Technology
- Biotechnology
- Foodservice
- Sustainability
---
