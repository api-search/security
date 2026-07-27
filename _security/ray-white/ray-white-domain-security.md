---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: raywhite.com
  spf: true
- caa: []
  dmarc: true
  dmarc_delegated: _dmarc.rwc.com.au.dmarc.has.pphosted.com
  dmarc_policy: reject
  dnssec: false
  domain: rwc.com.au
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all
- caa: []
  dmarc: true
  dmarc_delegated: _dmarc.nurturecloud.com.dmarc.has.pphosted.com
  dmarc_policy: reject
  dnssec: false
  domain: nurturecloud.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: auctionslive.com
  spf: true
  spf_record: v=spf1 a mx include:_spf.mlsend.com ?all
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  edge: CloudFront + nginx (Craft CMS)
  host: www.raywhite.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: rwc.com.au
  hsts: false
  https: true
  note: Ray White Commercial; HTTP 301 to canonical then 200
  tls_version: TLSv1.3
- host: nurturecloud.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: NurtureCloud, the group's proprietary agent platform
  tls_version: TLSv1.3
- host: auctionslive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ray White Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ray White, probed live across 4 host(s) and 4 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ray White
provider_slug: ray-white
slug: ray-white-domain-security
source_filename: ray-white-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + review.yml hosts\nnote: |\n  Ray White operates no API host, so these are the group's public web properties.\n  The raywhite.com edge (CloudFront + nginx + Craft CMS) returns 403 to default\n  curl User-Agents; the HSTS reading below was taken with a desktop Chrome\n  User-Agent, which is why it corrects the automated probe's null. DMARC for\n  rwc.com.au and nurturecloud.com is delegated via CNAME to Proofpoint\n  (_dmarc.<domain>.dmarc.has.pphosted.com) and resolves to p=reject.\nhosts:\n- host: www.raywhite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  edge: CloudFront + nginx (Craft CMS)\n- host: rwc.com.au\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: Ray White Commercial; HTTP 301 to canonical then 200\n- host: nurturecloud.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: NurtureCloud, the group's proprietary agent platform\n- host: auctionslive.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\ndomains:\n- domain: raywhite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rwc.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_delegated: _dmarc.rwc.com.au.dmarc.has.pphosted.com\n- domain: nurturecloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_delegated: _dmarc.nurturecloud.com.dmarc.has.pphosted.com\n- domain: auctionslive.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 a mx include:_spf.mlsend.com ?all\n  dmarc: false\n  dmarc_policy: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ray-white/refs/heads/main/security/ray-white-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Australia
- Brokerage
- Property Listings
- Property Management
- Rentals
- Commercial Real Estate
- Auctions
- Valuation
- PropTech
- Conveyancing
- Mortgage
---
