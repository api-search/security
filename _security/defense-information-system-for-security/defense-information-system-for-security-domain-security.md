---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dcsa.mil
  spf: true
hosts:
- cert_expires: Nov  2 19:35:49 2026 GMT
  host: www.dcsa.mil
  hsts: max-age=31536000
  hsts_note: HSTS header observed directly on the Akamai edge response (2026-09-07). The automated prober records null because every request to www.dcsa.mil — from two independent networks, with browser User-Agent and full browser headers — returns HTTP 403 "AkamaiGHost / Access Denied" instead of a page.
  http_status: 403
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Defense Information System For Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Information System for Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Information System for Security
provider_slug: defense-information-system-for-security
slug: defense-information-system-for-security-domain-security
source_filename: defense-information-system-for-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dcsa.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:35:49 2026 GMT\n  hsts: max-age=31536000\n  http_status: 403\n  hsts_note: >-\n    HSTS header observed directly on the Akamai edge response (2026-09-07). The\n    automated prober records null because every request to www.dcsa.mil — from\n    two independent networks, with browser User-Agent and full browser headers —\n    returns HTTP 403 \"AkamaiGHost / Access Denied\" instead of a page.\ndomains:\n- domain: dcsa.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-information-system-for-security/refs/heads/main/security/defense-information-system-for-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Defense
- Department of Defense
- DCSA
- Personnel Security
- Suitability
- Credentialing
- Security Clearance
- System of Record
---
