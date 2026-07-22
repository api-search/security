---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: federallabs.org
  spf: true
hosts:
- cert_expires: Sep  9 22:31:45 2026 GMT
  host: www.federallabs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Laboratory Consortium For Technology Transfer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Laboratory Consortium for Technology Transfer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Federal Laboratory Consortium for Technology Transfer
provider_slug: federal-laboratory-consortium-for-technology-transfer
slug: federal-laboratory-consortium-for-technology-transfer-domain-security
source_filename: federal-laboratory-consortium-for-technology-transfer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.federallabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:31:45 2026 GMT\n  hsts: false\ndomains:\n- domain: federallabs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-laboratory-consortium-for-technology-transfer/refs/heads/main/security/federal-laboratory-consortium-for-technology-transfer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Federal Government
- Technology Transfer
---
