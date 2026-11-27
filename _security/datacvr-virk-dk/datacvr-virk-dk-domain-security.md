---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: virk.dk
  spf: true
hosts:
- cert_expires: Jan 22 13:13:17 2027 GMT
  host: datacvr.virk.dk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CVR (Danish business register) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CVR (Danish business register), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CVR (Danish business register)
provider_slug: datacvr-virk-dk
slug: datacvr-virk-dk-domain-security
source_filename: datacvr-virk-dk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacvr.virk.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 13:13:17 2027 GMT\n  hsts: null\ndomains:\n- domain: virk.dk\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/datacvr-virk-dk/security/datacvr-virk-dk-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
