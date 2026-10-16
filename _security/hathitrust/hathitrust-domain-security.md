---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hathitrust.org
  spf: true
hosts:
- cert_expires: Dec 11 14:01:28 2026 GMT
  host: www.hathitrust.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hathitrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HathiTrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HathiTrust
provider_slug: hathitrust
slug: hathitrust-domain-security
source_filename: hathitrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hathitrust.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 14:01:28 2026 GMT\n  hsts: null\ndomains:\n- domain: hathitrust.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hathitrust/refs/heads/main/security/hathitrust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
