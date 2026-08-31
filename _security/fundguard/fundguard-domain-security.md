---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; pct=100; rua=mailto:dmarc_agg@vali.email,mailto:dmarc-report@fundguard.com
  dnssec: false
  domain: fundguard.com
  mta_sts: true
  mta_sts_mode: enforce
  mta_sts_policy: https://mta-sts.fundguard.com/.well-known/mta-sts.txt
  spf: true
  spf_all: -all
  spf_record: v=spf1 a mx ip4:35.188.91.53 include:_spf.google.com ... -all
hosts:
- cert_expires: Sep 15 09:23:39 2026 GMT
  host: www.fundguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  referrer_policy: strict-origin-when-cross-origin
  server: nginx
  tls_version: TLSv1.3
  x_content_type_options: nosniff
  x_frame_options: SAMEORIGIN
- content_security_policy: upgrade-insecure-requests
  host: kb.fundguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: HubSpot-hosted customer knowledge base behind a membership login
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fundguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FundGuard, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FundGuard
provider_slug: fundguard
slug: fundguard-domain-security
source_filename: fundguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fundguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:23:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: nginx\n  x_content_type_options: nosniff\n  x_frame_options: SAMEORIGIN\n  referrer_policy: strict-origin-when-cross-origin\n- host: kb.fundguard.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  server: cloudflare\n  content_security_policy: upgrade-insecure-requests\n  note: HubSpot-hosted customer knowledge base behind a membership login\ndomains:\n- domain: fundguard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; pct=100; rua=mailto:dmarc_agg@vali.email,mailto:dmarc-report@fundguard.com'\n  spf_record: v=spf1 a mx ip4:35.188.91.53 include:_spf.google.com ... -all\n  spf_all: '-all'\n  mta_sts: true\n\
  \  mta_sts_mode: enforce\n  mta_sts_policy: https://mta-sts.fundguard.com/.well-known/mta-sts.txt\nfindings:\n- id: dangling-cname\n  severity: observation\n  host: platform.fundguard.com\n  detail: >-\n    platform.fundguard.com is a CNAME to dr82nty150q0v.cloudfront.net, which resolves NOERROR with no A or\n    AAAA records - the referenced CloudFront distribution no longer exists. The hostname is therefore\n    unreachable and the record is dangling. Observed 2026-08-01 against 8.8.8.8 and the local resolver.\n- id: no-caa\n  severity: observation\n  domain: fundguard.com\n  detail: no CAA records published, so any public CA may issue for the domain\n- id: no-dnssec\n  severity: observation\n  domain: fundguard.com\n  detail: no DNSKEY present; the zone is not DNSSEC signed\n- id: strong-email-auth\n  severity: positive\n  domain: fundguard.com\n  detail: SPF ends in -all, DMARC p=reject pct=100 with aggregate reporting, and MTA-STS mode=enforce\nx-evidence:\n  fetched: '2026-08-01'\n\
  \  method: dig (@8.8.8.8 and local resolver), openssl s_client, curl HEAD\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundguard/refs/heads/main/security/fundguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- investment-accounting
- fund-accounting
- ibor
- abor
- nav
- asset-management
- portfolio-accounting
- private-markets
- Financial-Services
- Fintech
- saas
- artificial-intelligence
- MCP
---
