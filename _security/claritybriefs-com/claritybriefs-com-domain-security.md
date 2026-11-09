---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:info@claritybriefs.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: claritybriefs.com
  spf: true
hosts:
- cert_expires: Jan 17 17:09:20 2027 GMT
  host: claritybriefs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claritybriefs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for claritybriefs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: claritybriefs-com
provider_slug: claritybriefs-com
slug: claritybriefs-com-domain-security
source_filename: claritybriefs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claritybriefs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 17:09:20 2027 GMT\n  hsts: null\ndomains:\n- domain: claritybriefs.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:info@claritybriefs.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/claritybriefs-com/security/claritybriefs-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
