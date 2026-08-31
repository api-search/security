---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kuaecloud.net
  note: The KUAE Cloud API domain carries no SPF, no DMARC, no CAA and no DNSSEC — weaker than the mthreads.com corporate domain, which at least publishes SPF.
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: mthreads.com
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: www.mthreads.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: docs.mthreads.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- host: aibook-api.mthreads.com
  https: false
  note: Port 443 is closed on this host. The AIBook APIs are served on non-standard high ports (32414 TTS, 62220 ASR, 32314 voice conversion), each probed separately below.
- cert_valid: true
  host: aibook-api.mthreads.com:32414
  hsts: false
  https: true
  note: TTS. Handshake completes and the certificate chain validates; probes from the United States intermittently time out mid-handshake.
  tls_version: TLSv1.2
- cert_valid: true
  host: aibook-api.mthreads.com:62220
  hsts: false
  https: true
  note: ASR. Verified with an unauthenticated request returning HTTP 400 over a validated TLS 1.2 channel (ECDHE-RSA-AES128-GCM-SHA256).
  tls_version: TLSv1.2
- cert_valid: true
  host: aibook-api.mthreads.com:32314
  hsts: false
  https: true
  note: Streaming voice conversion.
  tls_version: TLSv1.2
- cert_valid: true
  host: coding-plan-endpoint.kuaecloud.net
  hsts: false
  https: true
  note: KUAE Cloud Coding Plan inference endpoint. Fronted by a Volcengine ALB (alb-xohaibke0f7k54ov5eie2tco.cn-beijing.volcenginealb.com). No Strict-Transport-Security header is returned, unlike the mthreads.com web hosts which set max-age=15724800.
kind: domain-security
layout: security
method: probed
name: Moore Threads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moore Threads, probed live across 7 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Moore Threads
provider_slug: moore-threads
slug: moore-threads-domain-security
source_filename: moore-threads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mthreads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.mthreads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: aibook-api.mthreads.com\n  https: false\n  note: >-\n    Port 443 is closed on this host. The AIBook APIs are served on non-standard high ports\n    (32414 TTS, 62220 ASR, 32314 voice conversion), each probed separately below.\n- host: 'aibook-api.mthreads.com:32414'\n  https: true\n  tls_version: TLSv1.2\n  cert_valid: true\n  hsts: false\n  note: TTS. Handshake completes and the certificate chain validates; probes from the United States intermittently time out mid-handshake.\n- host: 'aibook-api.mthreads.com:62220'\n  https: true\n  tls_version: TLSv1.2\n  cert_valid:\
  \ true\n  hsts: false\n  note: ASR. Verified with an unauthenticated request returning HTTP 400 over a validated TLS 1.2 channel (ECDHE-RSA-AES128-GCM-SHA256).\n- host: 'aibook-api.mthreads.com:32314'\n  https: true\n  tls_version: TLSv1.2\n  cert_valid: true\n  hsts: false\n  note: Streaming voice conversion.\n- host: coding-plan-endpoint.kuaecloud.net\n  https: true\n  cert_valid: true\n  hsts: false\n  note: >-\n    KUAE Cloud Coding Plan inference endpoint. Fronted by a Volcengine ALB\n    (alb-xohaibke0f7k54ov5eie2tco.cn-beijing.volcenginealb.com). No Strict-Transport-Security\n    header is returned, unlike the mthreads.com web hosts which set max-age=15724800.\ndomains:\n- domain: kuaecloud.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    The KUAE Cloud API domain carries no SPF, no DMARC, no CAA and no DNSSEC — weaker than the\n    mthreads.com corporate domain, which at least publishes SPF.\n- domain: mthreads.com\n  dnssec: false\n  caa: []\n  spf:\
  \ true\n  dmarc: false\nfindings:\n- The three AIBook API listeners run TLS 1.2 with no HSTS, while the marketing hosts run TLS 1.3 with HSTS — the API surface is the weaker half of the estate.\n- No host on either domain publishes CAA records, so any public CA may issue for mthreads.com or kuaecloud.net.\n- DNSSEC is unsigned on both domains and DMARC is absent on both.\nchecked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moore-threads/refs/heads/main/security/moore-threads-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- GPU
- Artificial Intelligence
- Machine-Learning
- Semiconductors
- Speech Recognition
- Text-to-Speech
- Voice
- LLM Inference
- Cloud Computing
- Developer Tools
- China
---
