---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: opensubtitles.com
  spf: true
hosts:
- cert_expires: Jan 11 03:31:41 2027 GMT
  host: opensubtitles.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opensubtitles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSubtitles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OpenSubtitles
provider_slug: opensubtitles
slug: opensubtitles-domain-security
source_filename: opensubtitles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensubtitles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 03:31:41 2027 GMT\n  hsts: null\ndomains:\n- domain: opensubtitles.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/opensubtitles/security/opensubtitles-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- subtitles
- video
- media
- API
---
