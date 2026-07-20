---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: insiderone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: useinsider.com
  spf: true
hosts:
- cert_expires: Sep  6 12:39:41 2026 GMT
  host: insiderone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 02:34:18 2026 GMT
  host: academy.insiderone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 03:30:39 2026 GMT
  host: unification.useinsider.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insider Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insider, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Insider
provider_slug: insider
slug: insider-domain-security
source_filename: insider-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insiderone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 12:39:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: academy.insiderone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:34:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: unification.useinsider.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:30:39 2026 GMT\n  hsts: null\ndomains:\n- domain: insiderone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: useinsider.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/security/insider-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Engagement
- Personalization
- Customer Data Platform
- Marketing
- Journey Orchestration
- Omnichannel
- CDP
- Artificial Intelligence
---
