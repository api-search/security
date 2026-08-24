---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jitjatjo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dayforceflexwork.com
  note: Successor domain carrying the production API hosts. Included because the Jitjatjo apps call it directly; not a separate company.
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com ip4:67.231.152.177 ip4:208.84.65.220 ip4:67.231.158.158 ip4:67.231.151.29 -all
hosts:
- host: www.jitjatjo.com
  https: false
  note: TLS handshake aborted by the Webflow edge (SSL alert 40) at TLS 1.1/1.2/1.3 and from every resolved IP. Canonical marketing site is unreachable.
- host: ondemandapi.dayforceflexwork.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  note: Production API host for the Jitjatjo "Ondemand" web app, read from the app's own JS bundle. On the acquirer's domain following the September 2025 Dayforce acquisition of JJJ International.
- host: jobs.jitjatjo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
- host: help.jitjatjo.com
  hsts: false
  https: true
  note: Intercom-hosted help center on a Jitjatjo custom domain; no HSTS header.
kind: domain-security
layout: security
method: probed
name: Jitjatjo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jitjatjo, probed live across 4 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS; 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jitjatjo
provider_slug: jitjatjo
slug: jitjatjo-domain-security
source_filename: jitjatjo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + production API hosts, 2026-08-23\nnote: >-\n  The headline finding is that the canonical marketing site is DOWN over HTTPS.\n  www.jitjatjo.com resolves to the Webflow edge (proxy-ssl.webflow.com) and that\n  edge aborts the TLS handshake with alert 40 (handshake_failure) on all three\n  of its IPs and at every offered TLS version, so no HTTPS request completes at\n  all. The apex jitjatjo.com 301s to it, and news.jitjatjo.com and\n  www.networkplatform.com sit behind the same Webflow edge with the same\n  failure. The Internet Archive's last successful capture of the site is\n  2026-06-08, which brackets when it broke. The product hosts are healthy —\n  the CloudFront apps and the production API host all negotiate TLS cleanly and\n  the API host sets HSTS.\nhosts:\n- host: www.jitjatjo.com\n  https: false\n  note: >-\n    TLS handshake aborted by the Webflow edge (SSL alert 40) at TLS 1.1/1.2/1.3\n\
  \    and from every resolved IP. Canonical marketing site is unreachable.\n- host: ondemandapi.dayforceflexwork.com\n  https: true\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n  note: >-\n    Production API host for the Jitjatjo \"Ondemand\" web app, read from the app's\n    own JS bundle. On the acquirer's domain following the September 2025 Dayforce\n    acquisition of JJJ International.\n- host: jobs.jitjatjo.com\n  https: true\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n- host: help.jitjatjo.com\n  https: true\n  hsts: false\n  note: Intercom-hosted help center on a Jitjatjo custom domain; no HSTS header.\ndomains:\n- domain: jitjatjo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dayforceflexwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 include:spf.protection.outlook.com ip4:67.231.152.177\n    ip4:208.84.65.220 ip4:67.231.158.158 ip4:67.231.151.29\
  \ -all\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    Successor domain carrying the production API hosts. Included because the\n    Jitjatjo apps call it directly; not a separate company.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitjatjo/refs/heads/main/security/jitjatjo-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- Staffing
- Human Resources
- Workforce Management
- Talent Marketplace
- Gig Economy
- Contingent Labor
- Vendor Management
- Hospitality
- Healthcare Staffing
---
