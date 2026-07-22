---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=5; fo=1;
  dnssec: false
  domain: eclypsium.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:5610435.spf07.hubspotemail.net include:mail.zendesk.com ~all
hosts:
- host: eclypsium.com
  hsts: null
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eclypsium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eclypsium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eclypsium
provider_slug: eclypsium
slug: eclypsium-domain-security
source_filename: eclypsium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: dig + TLS/HTTP probe of eclypsium.com\nhosts:\n  - host: eclypsium.com\n    https: true\n    tls_version: TLSv1.3\n    hsts: null            # main site behind bot protection (HTTP 403 to HEAD); HSTS header not observable\n    hsts_max_age: null\ndomains:\n  - domain: eclypsium.com\n    dnssec: false         # no DNSKEY records\n    caa:\n      - '0 issue \"amazon.com\"'\n      - '0 issue \"amazonaws.com\"'\n      - '0 issue \"amazontrust.com\"'\n      - '0 issue \"awstrust.com\"'\n      - '0 issue \"comodoca.com\"'\n      - '0 issue \"digicert.com; cansignhttpexchanges=yes\"'\n      - '0 issue \"letsencrypt.org\"'\n      - '0 issue \"pki.goog; cansignhttpexchanges=yes\"'\n      - '0 issue \"ssl.com\"'\n    spf: true\n    spf_record: 'v=spf1 include:_spf.google.com include:5610435.spf07.hubspotemail.net include:mail.zendesk.com ~all'\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_record: 'v=DMARC1; p=quarantine; pct=5;\
  \ fo=1;'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclypsium/refs/heads/main/security/eclypsium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Firmware Security
- Supply Chain Security
- Hardware Security
- Infrastructure Security
- Endpoint Security
- Threat Detection
---
