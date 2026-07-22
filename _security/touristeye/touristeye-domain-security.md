---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: touristeye.com
  domain_created: '2009-10-19'
  domain_expires: '2026-10-19'
  note: whois lists AWS Route 53 nameservers and an active registration, but the delegated nameservers return no records for the zone (no A/NS/SOA/MX). The domain is registered but dark — the TouristEye service is defunct (last archive.org snapshot of the live site is from 2016; by 2017 the site was a 301 redirect).
  registered: true
  registrar: GoDaddy Corporate Domains, LLC
  spf: false
  whois_nameservers:
  - ns-1353.awsdns-41.org
  - ns-635.awsdns-15.net
  - ns-1725.awsdns-23.co.uk
hosts:
- host: touristeye.com
  hsts: null
  https: false
  note: curl exit 6 (could not resolve host); no A record published
  resolves: false
  tls_version: null
- host: www.touristeye.com
  hsts: null
  https: false
  resolves: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Touristeye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TouristEye, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TouristEye
provider_slug: touristeye
slug: touristeye-domain-security
source_filename: touristeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (dig, curl, whois; domain does not resolve)\nhosts:\n- host: touristeye.com\n  resolves: false\n  https: false\n  tls_version: null\n  hsts: null\n  note: curl exit 6 (could not resolve host); no A record published\n- host: www.touristeye.com\n  resolves: false\n  https: false\n  tls_version: null\n  hsts: null\ndomains:\n- domain: touristeye.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  registered: true\n  registrar: GoDaddy Corporate Domains, LLC\n  domain_created: '2009-10-19'\n  domain_expires: '2026-10-19'\n  whois_nameservers:\n  - ns-1353.awsdns-41.org\n  - ns-635.awsdns-15.net\n  - ns-1725.awsdns-23.co.uk\n  note: whois lists AWS Route 53 nameservers and an active registration, but the\n    delegated nameservers return no records for the zone (no A/NS/SOA/MX). The\n    domain is registered but dark — the TouristEye service is defunct (last\n\
  \    archive.org snapshot of the live site is from 2016; by 2017 the site was a\n    301 redirect).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/touristeye/refs/heads/main/security/touristeye-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Travel
- Trip Planning
- Mobile Apps
- Consumer
- Defunct
---
