---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@digitalocean.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digitalocean.com
  spf: true
hosts:
- cert_expires: Sep 25 14:26:22 2026 GMT
  host: status.digitalocean.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digitalocean Status Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigitalOcean Status, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DigitalOcean Status
provider_slug: digitalocean-status
slug: digitalocean-status-domain-security
source_filename: digitalocean-status-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: status.digitalocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:26:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: digitalocean.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@digitalocean.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitalocean-status/refs/heads/main/security/digitalocean-status-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development
- Public APIs
---
