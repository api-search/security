---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dalma.co
  spf: true
hosts:
- cert_expires: Oct 14 09:11:08 2026 GMT
  host: www.dalma.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dalma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dalma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dalma
provider_slug: dalma
slug: dalma-domain-security
source_filename: dalma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dalma.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:11:08 2026 GMT\n  hsts: false\ndomains:\n- domain: dalma.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dalma/refs/heads/main/security/dalma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Insurance
- InsurTech
- Pet Insurance
- Pets
- Veterinary
- France
---
