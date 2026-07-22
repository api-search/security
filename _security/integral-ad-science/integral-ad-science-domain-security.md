---
description: ''
domains:
- caa:
  - wp.wpenginepowered.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: integralads.com
  spf: true
hosts:
- cert_expires: Sep 30 19:51:35 2026 GMT
  host: integralads.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Integral Ad Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Integral Ad Science, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Integral Ad Science
provider_slug: integral-ad-science
slug: integral-ad-science-domain-security
source_filename: integral-ad-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: integralads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:51:35 2026 GMT\n  hsts: false\ndomains:\n- domain: integralads.com\n  dnssec: true\n  caa:\n  - wp.wpenginepowered.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integral-ad-science/refs/heads/main/security/integral-ad-science-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Advertising
- Ad Verification
- Ad Measurement
- Brand Safety
- Ad Fraud
- Viewability
- Contextual Targeting
- Attention Measurement
- CTV
- Connected TV
- Video Advertising
- Programmatic
- Header Bidding
- Prebid
- AdTech
- Marketing
- Media Quality
---
