---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marleymedical.com
  spf: true
hosts:
- host: www.marleymedical.com
  https: false
  platform: webflow
  tls_note: TLS handshake failure (server rejected ClientHello from probe clients)
- host: marleymedical.com
  https: false
  platform: netlify
  tls_note: apex record (75.2.70.75) returned TLS internal_error alert to probe clients
- host: my.marleymedical.com
  https: false
  platform: netlify
  tls_note: patient portal; TLS handshake failure from probe clients
kind: domain-security
layout: security
method: probed
name: Marley Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marley Medical, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marley Medical
provider_slug: marley-medical
slug: marley-medical-domain-security
source_filename: marley-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS probes of apis.yml website + email hosts (July 2026)\nnotes: >-\n  Marley Medical's public web endpoints (Webflow marketing/signup and a Netlify-hosted\n  patient portal) rejected the TLS ClientHello from every non-browser probe client\n  (OpenSSL, LibreSSL, and Python), so HTTPS reachability and HSTS could not be observed\n  programmatically; the sites do serve to real browsers. DNS-layer records below were\n  resolved successfully with dig.\nhosts:\n- host: www.marleymedical.com\n  platform: webflow\n  https: false\n  tls_note: TLS handshake failure (server rejected ClientHello from probe clients)\n- host: marleymedical.com\n  platform: netlify\n  https: false\n  tls_note: apex record (75.2.70.75) returned TLS internal_error alert to probe clients\n- host: my.marleymedical.com\n  platform: netlify\n  https: false\n  tls_note: patient portal; TLS handshake failure from probe clients\ndomains:\n- domain: marleymedical.com\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marley-medical/refs/heads/main/security/marley-medical-domain-security.yml
summary_line: DMARC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Digital Health
- Virtual Care
- Medical
---
