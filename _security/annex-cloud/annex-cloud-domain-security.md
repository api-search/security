---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: annexcloud.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: redocly.app
  spf: false
hosts:
- cert_expires: Sep 24 11:03:51 2026 GMT
  host: www.annexcloud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 04:58:02 2026 GMT
  host: annexcloud.redocly.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Annex Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Annex Cloud, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Annex Cloud
provider_slug: annex-cloud
slug: annex-cloud-domain-security
source_filename: annex-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.annexcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:03:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: annexcloud.redocly.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:58:02 2026 GMT\n  hsts: false\ndomains:\n- domain: annexcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: redocly.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/annex-cloud/refs/heads/main/security/annex-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Customer Retention
- Rewards
- Points
- Referrals
- Customer Engagement
- Enterprise
- Gated Access
---
