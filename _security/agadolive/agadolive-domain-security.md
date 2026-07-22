---
description: ''
domains:
- caa:
  - 0 iodef "mailto:support@agadolive.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agadolive.com
  spf: true
hosts:
- cert_expires: Sep 14 14:20:31 2026 GMT
  host: agadolive.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agadolive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgadoLive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AgadoLive
provider_slug: agadolive
slug: agadolive-domain-security
source_filename: agadolive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agadolive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:20:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: agadolive.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:support@agadolive.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agadolive/refs/heads/main/security/agadolive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Telehealth
- Rehabilitation
- Physical Therapy
- Computer Vision
- Artificial Intelligence
- Healthcare
---
