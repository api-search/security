---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blobr.io
  spf: true
hosts:
- cert_expires: Aug 15 06:45:29 2026 GMT
  host: www.blobr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blobr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blobr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blobr
provider_slug: blobr
slug: blobr-domain-security
source_filename: blobr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blobr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 06:45:29 2026 GMT\n  hsts: null\ndomains:\n- domain: blobr.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blobr/refs/heads/main/security/blobr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- AI Agents
- Google Ads
- Marketing Automation
- PPC
---
