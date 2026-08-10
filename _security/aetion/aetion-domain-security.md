---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aetion.com
  spf: true
hosts:
- cert_expires: Oct 20 18:17:57 2026 GMT
  host: aetion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'aetion.com and www.aetion.com both answer HTTP 301 (HubSpot-managed redirects behind Cloudflare) and send strict-transport-security: max-age=31536000 on the redirect response. The apex 301s to https://www.datavant.com/ following the Datavant acquisition, so no Aetion-origin content is served from this host.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aetion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aetion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aetion
provider_slug: aetion
slug: aetion-domain-security
source_filename: aetion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aetion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 18:17:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    aetion.com and www.aetion.com both answer HTTP 301 (HubSpot-managed redirects behind\n    Cloudflare) and send strict-transport-security: max-age=31536000 on the redirect\n    response. The apex 301s to https://www.datavant.com/ following the Datavant\n    acquisition, so no Aetion-origin content is served from this host.\ndomains:\n- domain: aetion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aetion/refs/heads/main/security/aetion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-World Evidence
- Healthcare
- Life Sciences
- Clinical Research
- Health Data
- Data Analytics
---
