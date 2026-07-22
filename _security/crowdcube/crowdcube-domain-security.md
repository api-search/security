---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crowdcube.com
  spf: true
hosts:
- cert_expires: Sep 20 17:23:40 2026 GMT
  host: www.crowdcube.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crowdcube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crowdcube, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: crowdcube
provider_slug: crowdcube
slug: crowdcube-domain-security
source_filename: crowdcube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowdcube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:23:40 2026 GMT\n  hsts: null\ndomains:\n- domain: crowdcube.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdcube/refs/heads/main/security/crowdcube-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Equity Crowdfunding
- Investing
- Fintech
- Startups
- Fundraising
- United Kingdom
---
