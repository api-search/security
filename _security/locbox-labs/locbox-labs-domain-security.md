---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hownd.com
  spf: true
hosts:
- cert_expires: Oct 26 12:52:46 2026 GMT
  host: hownd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: partner-api.hownd.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Locbox Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocBox Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LocBox Labs
provider_slug: locbox-labs
slug: locbox-labs-domain-security
source_filename: locbox-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hownd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 12:52:46 2026 GMT\n  hsts: false\n- host: partner-api.hownd.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hownd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locbox-labs/refs/heads/main/security/locbox-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Promotions
- Local Marketing
- Small Business
- Automation
- Coupons
- Email Marketing
- Loyalty
- Guest WiFi
- Family Entertainment
- Restaurants
---
