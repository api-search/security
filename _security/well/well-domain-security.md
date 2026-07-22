---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "rapidssl.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: well.co
  spf: true
hosts:
- cert_expires: Sep 29 17:45:47 2026 GMT
  host: www.well.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Well Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Well, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Well
provider_slug: well
slug: well-domain-security
source_filename: well-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.well.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:45:47 2026 GMT\n  hsts: false\ndomains:\n- domain: well.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/well/refs/heads/main/security/well-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Digital Health
- Health Engagement
- Wellness
- Wellbeing
- Employee Benefits
---
