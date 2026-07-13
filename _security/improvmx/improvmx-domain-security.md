---
description: ''
domains:
- caa:
  - 128 iodef "mailto:support@improvmx.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: improvmx.com
  spf: true
hosts:
- cert_expires: Aug 31 05:59:27 2026 GMT
  host: improvmx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Improvmx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImprovMX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ImprovMX
provider_slug: improvmx
slug: improvmx-domain-security
source_filename: improvmx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: improvmx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:59:27 2026 GMT\n  hsts: false\ndomains:\n- domain: improvmx.com\n  dnssec: true\n  caa:\n  - 128 iodef \"mailto:support@improvmx.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/improvmx/refs/heads/main/security/improvmx-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- Public APIs
---
