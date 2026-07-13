---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Rewardful REST API
  slug: rewardful-rest-api
  spec_type: OpenAPI
  url: https://developers.rewardful.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rewardful.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getrewardful.com
  spf: true
hosts:
- cert_expires: Aug 17 01:45:22 2026 GMT
  host: www.rewardful.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:05:13 2026 GMT
  host: developers.rewardful.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 02:01:09 2026 GMT
  host: api.getrewardful.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rewardful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rewardful, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rewardful
provider_slug: rewardful
slug: rewardful-domain-security
source_filename: rewardful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rewardful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 01:45:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.rewardful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:05:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getrewardful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:01:09 2026 GMT\n  hsts: null\ndomains:\n- domain: rewardful.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getrewardful.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rewardful/refs/heads/main/security/rewardful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Tracking
- Referral Programs
- SaaS
- Stripe
- Commissions
- Payouts
---
