---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:rua@dmarc.brevo.com
  dnssec: false
  domain: kneron.com
  notes: No SPF record on kneron.com (only a site-verification TXT and a Brevo verification code). No CAA. No DNSSEC. DMARC is published but at p=none (monitor only). No host sends HSTS; www.kneron.com and doc.kneron.com negotiate TLS 1.2 only, while kneo.kneron.com and kneoedge.kneron.com negotiate TLS 1.3.
  spf: false
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.kneron.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: doc.kneron.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: kneo.kneron.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: kneoedge.kneron.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kneron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kneron, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Kneron
provider_slug: kneron
slug: kneron-domain-security
source_filename: kneron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kneron.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: doc.kneron.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\n- host: kneo.kneron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: kneoedge.kneron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kneron.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: 'v=DMARC1; p=none; rua=mailto:rua@dmarc.brevo.com'\n  notes: >-\n    No SPF record on kneron.com (only a site-verification TXT and a Brevo\n    verification code). No CAA. No DNSSEC. DMARC is published but at p=none\n    (monitor only). No host sends HSTS; www.kneron.com\
  \ and doc.kneron.com\n    negotiate TLS 1.2 only, while kneo.kneron.com and kneoedge.kneron.com\n    negotiate TLS 1.3.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kneron/refs/heads/main/security/kneron-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- Edge AI
- Semiconductors
- Neural Processing Unit
- Machine Learning
- Computer Vision
- AIoT
- Hardware
- Large Language Models
- On-Premise AI
- SDK
- Embedded Systems
---
