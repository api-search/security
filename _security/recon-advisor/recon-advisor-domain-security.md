---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ipacket.us
  spf: true
hosts:
- cert_expires: Feb 12 00:27:19 2027 GMT
  host: ipacket.us
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AutoIPacket, LLC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoIPacket, LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AutoIPacket, LLC
provider_slug: recon-advisor
slug: recon-advisor-domain-security
source_filename: recon-advisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipacket.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 00:27:19 2027 GMT\n  hsts: false\ndomains:\n- domain: ipacket.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/recon-advisor/security/recon-advisor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- DealerTech
- VehicleReconditioning
- Software-as-a-Service
- AutoIPacket
---
