---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onetext.com
  spf: true
hosts:
- cert_expires: Jan  7 13:52:56 2027 GMT
  host: home.onetext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onetext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneText, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OneText
provider_slug: onetext
slug: onetext-domain-security
source_filename: onetext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.onetext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:52:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onetext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onetext/security/onetext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text to Buy
- Ecommerce
- SMS Marketing
- Conversational Sales
- AI Smart Replies
- Payments
- Cart Recovery
---
