---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aiforcetech.com
  note: No _dmarc.aiforcetech.com TXT record and no CAA record at the apex. Mail is Alibaba Cloud (mxhichina.com).
  spf: true
  spf_record: v=spf1 include:spf.mxhichina.com -all
hosts:
- cert_expires: Oct  2 02:23:46 2026 GMT
  cert_issuer: Let's Encrypt (YE1)
  host: www.aiforcetech.com
  hsts: null
  https: true
  note: HSTS could not be read — the Alibaba Cloud (Tengine/kunlun) edge answered every HEAD/GET with HTTP 429 after the first handful of probes, so no response headers were observable. Recorded as unknown rather than false.
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiforcetech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIForce Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AIForce Technology
provider_slug: aiforcetech
slug: aiforcetech-domain-security
source_filename: aiforcetech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the aiforcetech.com marketing host (the company publishes\n  no API host); TLS values read directly with openssl s_client after probe-domain-security.py\n  recorded a transient socket failure against the Alibaba Cloud CDN edge.\nhosts:\n- host: www.aiforcetech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt (YE1)\"\n  cert_expires: Oct  2 02:23:46 2026 GMT\n  hsts: null\n  note: HSTS could not be read — the Alibaba Cloud (Tengine/kunlun) edge answered every\n    HEAD/GET with HTTP 429 after the first handful of probes, so no response headers\n    were observable. Recorded as unknown rather than false.\ndomains:\n- domain: aiforcetech.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.mxhichina.com -all\n  dmarc: false\n  note: No _dmarc.aiforcetech.com TXT record and no CAA record at the apex. Mail is\n    Alibaba Cloud (mxhichina.com).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiforcetech/refs/heads/main/security/aiforcetech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agriculture
- Agricultural Machinery
- Agricultural Robotics
- Robotics
- Artificial Intelligence
- Autonomous Vehicles
- Precision Agriculture
- Electric Vehicles
- China
---
