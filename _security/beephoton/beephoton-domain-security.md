---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: beephoton.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: beephoton.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beephoton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beephoton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Beephoton
provider_slug: beephoton
slug: beephoton-domain-security
source_filename: beephoton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beephoton.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: beephoton.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beephoton/refs/heads/main/security/beephoton-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- PhotonDetection
- Medical Imaging
- Industrial
- Security
---
