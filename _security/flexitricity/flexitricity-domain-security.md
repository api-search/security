---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc@flexitricity.com; sp=quarantine; adkim=r; aspf=r;
  dnssec: false
  domain: flexitricity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc@flexitricity.com; sp=quarantine; adkim=r; aspf=r;
  dnssec: false
  domain: flexgo.energy
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:144179153.spf01.hubspotemail.net -all
hosts:
- cert_expires: Jan 28 11:46:20 2027 GMT
  host: www.flexitricity.com
  hsts: false
  https: true
  note: Marketing site (Next.js). No HSTS header on the primary marketing host.
  tls_version: TLSv1.3
- cert_expires: Jan 28 11:46:20 2027 GMT
  host: portal.flexitricity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Customer portal. Two-year HSTS. Every path auth-walls to /login.
  tls_version: TLSv1.3
- host: cms.flexitricity.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Headless CMS (Strapi). A content API exists at /api but every collection returns 403 Forbidden to the anonymous public role; /_health returns 204.
  tls_version: TLSv1.3
- host: flexgo.energy
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: FlexGO product site on a separate domain (A record 20.90.217.7).
  tls_version: TLSv1.3
- host: www.flexgo.energy
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: trading.flexitricity.com
  https: false
  note: DANGLING CNAME. trading.flexitricity.com returns CNAME dhenfu8l1wx2e.cloudfront.net from the local resolver, 1.1.1.1 and 8.8.8.8, but that CloudFront name itself has no address records — the distribution it points at no longer exists, so no connection is possible ("Could not resolve host"). Recorded as observed DNS state on 2026-07-27. An unclaimed CNAME target of this shape is the classic subdomain-takeover precondition.
  resolves: false
kind: domain-security
layout: security
method: probed
name: Flexitricity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexitricity, probed live across 6 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flexitricity
provider_slug: flexitricity
slug: flexitricity-domain-security
source_filename: flexitricity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Flexitricity-operated host in apis.yml plus\n  a subdomain sweep (this provider publishes no OpenAPI, so there are no servers[]\n  hosts to probe)\nhosts:\n- host: www.flexitricity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 11:46:20 2027 GMT\n  hsts: false\n  note: Marketing site (Next.js). No HSTS header on the primary marketing host.\n- host: portal.flexitricity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 11:46:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Customer portal. Two-year HSTS. Every path auth-walls to /login.\n- host: cms.flexitricity.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Headless CMS (Strapi). A content API exists at /api but every collection\n    returns 403 Forbidden to the anonymous public role; /_health returns 204.\n- host: flexgo.energy\n\
  \  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: FlexGO product site on a separate domain (A record 20.90.217.7).\n- host: www.flexgo.energy\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: trading.flexitricity.com\n  https: false\n  resolves: false\n  note: DANGLING CNAME. trading.flexitricity.com returns CNAME\n    dhenfu8l1wx2e.cloudfront.net from the local resolver, 1.1.1.1 and 8.8.8.8, but\n    that CloudFront name itself has no address records — the distribution it points\n    at no longer exists, so no connection is possible (\"Could not resolve host\").\n    Recorded as observed DNS state on 2026-07-27. An unclaimed CNAME target of this\n    shape is the classic subdomain-takeover precondition.\ndomains:\n- domain: flexitricity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1;\
  \ p=quarantine; pct=100; rua=mailto:dmarc@flexitricity.com;\n    sp=quarantine; adkim=r; aspf=r;'\n- domain: flexgo.energy\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:144179153.spf01.hubspotemail.net\n    -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc@flexitricity.com;\n    sp=quarantine; adkim=r; aspf=r;'\nsummary:\n  tls: Every reachable host negotiates TLSv1.3 with a valid certificate.\n  hsts: Present on the portal, CMS and FlexGO hosts; absent on the primary www\n    marketing host.\n  dnssec: Not enabled on either domain.\n  caa: No CAA records published on either domain.\n  email_auth: SPF and DMARC published on both domains; DMARC policy is quarantine\n    (not reject) with aggregate reporting to dmarc@flexitricity.com.\n  observations:\n  - One dangling CNAME (trading.flexitricity.com -> a non-resolving CloudFront\n    distribution).\n  - No security.txt\
  \ is served on any host (see well-known/flexitricity-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexitricity/refs/heads/main/security/flexitricity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Demand Response
- Energy Markets
- Grid
- DER
- Battery Storage
- Virtual Power Plant
- Flexibility
- EV Charging
---
