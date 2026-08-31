---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: woebothealth.com
  spf: true
hosts:
- cert_expires: Aug 31 08:08:20 2026 GMT
  host: woebothealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Woebot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Woebot Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Woebot Health
provider_slug: woebot
slug: woebot-domain-security
source_filename: woebot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woebothealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:08:20 2026 GMT\n  hsts: false\ndomains:\n- domain: woebothealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woebot/refs/heads/main/security/woebot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mental Health
- Digital Therapeutics
- CBT
- Chatbot
- Clinical
- Healthcare
- B2B
- Enterprise
---
