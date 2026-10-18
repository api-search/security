---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: cosmocloud.io
  spf: true
hosts:
- cert_expires: Nov 20 07:24:15 2026 GMT
  host: cosmocloud.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosmiccloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmiccloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cosmiccloud
provider_slug: cosmiccloud
slug: cosmiccloud-domain-security
source_filename: cosmiccloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cosmocloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 07:24:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cosmocloud.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmiccloud/refs/heads/main/security/cosmiccloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud
- DevOps
- Automation
- Deployment
- Startups
- Company
---
