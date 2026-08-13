---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kling.ai
  note: DMARC p=none and sp=none — monitoring only, no enforcement, on the domain that hosts the OAuth authorization server and the MCP endpoint.
  probed: '2026-08-12'
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klingai.com
  note: Fronted by Akamai (wildcard.klingai.com.edgesuite.net).
  probed: '2026-08-12'
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kuaishou.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kwai.com
  spf: true
hosts:
- cert_expires: Feb 26 06:51:24 2027 GMT
  host: www.kuaishou.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  7 03:46:08 2026 GMT
  host: open.kuaishou.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 08:23:34 2026 GMT
  host: developers.kwai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:05:22 2026 GMT
  host: kling.ai
  hsts: partial
  hsts_note: 'The document root does NOT send Strict-Transport-Security, but the application endpoints do: https://kling.ai/mcp returns "strict-transport-security: max-age=31536000 ; includeSubDomains". HSTS is therefore inconsistent across the same host, which is a real weakness — a first visit to kling.ai is not protected.'
  https: true
  probed: '2026-08-12'
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:20:21 2026 GMT
  host: api-singapore.klingai.com
  hsts: false
  https: true
  probed: '2026-08-12'
  tls_version: TLSv1.3
- cert_expires: Jan 24 08:07:33 2027 GMT
  host: api-beijing.klingai.com
  hsts: false
  https: true
  note: The China API endpoint did not negotiate TLS 1.3 while the Singapore endpoint did.
  probed: '2026-08-12'
  tls13_supported: false
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kuaishou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuaishou, probed live across 6 host(s) and 4 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kuaishou
provider_slug: kuaishou
slug: kuaishou-domain-security
source_filename: kuaishou-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (0-working/probe-domain-security.py, 2026-08-12),\n  plus manual TLS/DNS probes of the Kling AI hosts on 2026-08-12\nhosts:\n- host: www.kuaishou.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 06:51:24 2027 GMT\n  hsts: false\n- host: open.kuaishou.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 03:46:08 2026 GMT\n  hsts: false\n- host: developers.kwai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:23:34 2026 GMT\n  hsts: false\n- host: kling.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:05:22 2026 GMT\n  hsts: partial\n  hsts_note: >-\n    The document root does NOT send Strict-Transport-Security, but the application endpoints do:\n    https://kling.ai/mcp returns \"strict-transport-security: max-age=31536000 ; includeSubDomains\".\n    HSTS is therefore inconsistent across the same\
  \ host, which is a real weakness — a first visit to\n    kling.ai is not protected.\n  probed: '2026-08-12'\n- host: api-singapore.klingai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:20:21 2026 GMT\n  hsts: false\n  probed: '2026-08-12'\n- host: api-beijing.klingai.com\n  https: true\n  tls_version: TLSv1.2\n  tls13_supported: false\n  cert_expires: Jan 24 08:07:33 2027 GMT\n  hsts: false\n  probed: '2026-08-12'\n  note: The China API endpoint did not negotiate TLS 1.3 while the Singapore endpoint did.\ndomains:\n- domain: kling.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: none\n  probed: '2026-08-12'\n  note: >-\n    DMARC p=none and sp=none — monitoring only, no enforcement, on the domain that hosts the OAuth\n    authorization server and the MCP endpoint.\n- domain: klingai.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc:\
  \ true\n  dmarc_policy: reject\n  probed: '2026-08-12'\n  note: Fronted by Akamai (wildcard.klingai.com.edgesuite.net).\n- domain: kuaishou.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kwai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuaishou/refs/heads/main/security/kuaishou-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Social
- Video
- Short Video
- Live Streaming
- Advertising
- Marketing
- Social Media
- Content
- China
- AI
- Generative AI
- Machine Learning
- MCP
---
