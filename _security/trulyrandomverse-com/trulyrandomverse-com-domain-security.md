---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: trulyrandomverse.com
  spf: true
hosts:
- cert_expires: Feb 12 17:03:21 2027 GMT
  host: trulyrandomverse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Truly Random Verse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truly Random Verse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truly Random Verse
provider_slug: trulyrandomverse-com
slug: trulyrandomverse-com-domain-security
source_filename: trulyrandomverse-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trulyrandomverse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 17:03:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trulyrandomverse.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trulyrandomverse-com/security/trulyrandomverse-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bible
- Religion
- Study Tools
- AI
- Open Source
---
